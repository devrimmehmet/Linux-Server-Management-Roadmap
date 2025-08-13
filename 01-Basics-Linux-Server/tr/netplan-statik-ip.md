# Ubuntu 24.04'te Netplan ile Sabit IP Ayarlama

Bu rehber, Ubuntu 24.04.3 LTS sunucuda Netplan kullanarak sabit (static) IP adresi ayarlamayı gösterir.

---

## 1. Netplan Nedir?

Netplan, Ubuntu’da ağ yapılandırmasını YAML formatında tanımlayarak kolayca yönetmemizi sağlayan bir araçtır.  
Yapılandırma dosyaları genellikle `/etc/netplan/` dizininde bulunur.

---

## 2. Ağ Arabirimini Öğrenme

    ip addr show

Örnek çıktı:
```
2: ens18: <BROADCAST,MULTICAST,UP,LOWER_UP> mtu 1500 qdisc fq_codel state UP group default qlen 1000
    inet 192.168.1.50/24 brd 192.168.1.255 scope global dynamic ens18
```

Burada **ens18** ağ arabirimi adıdır.

---

## 3. Mevcut Netplan Dosyasını Bulma

Netplan dosyaları genellikle:

    /etc/netplan/00-installer-config.yaml

veya

    /etc/netplan/01-netcfg.yaml

olarak bulunur.

Listelemek için:

    ls /etc/netplan/

---

## 4. Yedek Almak

Değişiklik yapmadan önce dosyayı yedekleyin:

    sudo cp /etc/netplan/00-installer-config.yaml /etc/netplan/00-installer-config.yaml.bak

---

## 5. Statik IP Yapılandırması

Dosyayı düzenleyin:

    sudo nano /etc/netplan/00-installer-config.yaml

Aşağıdaki örneğe göre düzenleyin (arabirim adınızı kendi sisteminizdeki ile değiştirin):

```
network:
  version: 2
  ethernets:
    ens18:
      dhcp4: no
      addresses:
        - 192.168.1.50/24
      gateway4: 192.168.1.1
      nameservers:
        addresses:
          - 8.8.8.8
          - 1.1.1.1
```

**Açıklamalar:**
- `ens18` → Ağ arabirimi adı
- `dhcp4: no` → DHCP kapatıldı, manuel IP kullanılacak
- `addresses` → Sabit IP adresi ve subnet maskesi
- `gateway4` → Varsayılan ağ geçidi
- `nameservers` → DNS sunucuları

---

## 6. Değişiklikleri Uygulamak

    sudo netplan apply

Eğer anlık hata kontrolü yapmak isterseniz:

    sudo netplan try

Bu komut 120 saniye içinde onay bekler, onaylamazsanız eski ayarlara döner.

---

## 7. Ayarları Doğrulama

    ip addr show ens18

veya

    ping 8.8.8.8 -c 4

---

## 8. Olası Hatalar ve Çözümleri

- **YAML format hatası** → Girintilere dikkat edin, boşluk kullanın, tab kullanmayın.
- **İnternet yok** → Gateway veya DNS adreslerini kontrol edin.
- **Yanlış arabirim adı** → `ip addr` ile doğru adı bulun.

---

✅ **Not:** Statik IP ayarını yaptıktan sonra SSH ile bağlanıyorsanız yeni IP adresini kullanarak tekrar bağlantı kurmanız gerekir.