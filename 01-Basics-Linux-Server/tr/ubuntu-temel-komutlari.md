# Ubuntu Temel Komutları

Bu döküman, Ubuntu 24.04.3 üzerinde günlük kullanımda en sık ihtiyaç duyacağınız komutların kısa bir özetidir.

## 1. Sistem Bilgileri
```bash
# Sistem bilgilerini göster
uname -a

# Dağıtım bilgilerini göster
lsb_release -a

# Donanım bilgileri
lshw -short

# CPU bilgisi
lscpu

# Bellek bilgisi
free -h

# Disk kullanım bilgisi
df -h
```

---

## 2. Dizin ve Dosya İşlemleri
```bash

# Dizin içeriğini listele
ls
ls -l      # detaylı liste
ls -la     # gizli dosyalar dahil

# Dizin değiştirme
cd /path/to/folder

# Dizin oluşturma
mkdir yeni_klasor

# Dosya oluşturma
touch yeni_dosya.txt

# Dosya/dizin kopyalama
cp kaynak.txt hedef.txt
cp -r kaynak_klasor hedef_klasor

# Dosya/dizin taşıma veya yeniden adlandırma
mv eski.txt yeni.txt

# Dosya/dizin silme
rm dosya.txt
rm -r klasor
```

---
## 3. Paket Yönetimi (APT)
```bash
# Paket listesini güncelle
sudo apt update

# Tüm paketleri yükselt
sudo apt upgrade -y

# Belirli bir paketi yükle
sudo apt install paket-adi

# Paketi kaldır
sudo apt remove paket-adi

# Paket hakkında bilgi
apt show paket-adi

# Paket arama
apt search kelime
```

---

## 4. Kullanıcı Yönetimi

```bash

# Yeni kullanıcı ekleme
sudo adduser kullaniciadi

# Kullanıcıyı sudo yetkisine ekleme
sudo usermod -aG sudo kullaniciadi

# Kullanıcı silme
sudo deluser kullaniciadi
```
---

## 5. Servis Yönetimi (systemctl)

```bash

# Servisi başlat
sudo systemctl start servisadi

# Servisi durdur
sudo systemctl stop servisadi

# Servisi yeniden başlat
sudo systemctl restart servisadi

# Servis durumunu görüntüle
systemctl status servisadi

# Servisin açılışta çalışmasını sağla
sudo systemctl enable servisadi

# Servisin açılışta çalışmasını engelle
sudo systemctl disable servisadi

```

---

## 6. Ağ Komutları

```bash

# IP adreslerini görüntüle
ip addr show

# Varsayılan ağ geçidini görüntüle
ip route show

# Belirli bir adrese ping at
ping google.com

# Açık portları listele
sudo lsof -i -P -n | grep LISTEN

# Netplan ayarlarını uygula
sudo netplan apply

```
---

## 7. Dosya İçerik İşlemleri

```bash

# Dosya içeriğini görüntüle
cat dosya.txt

# Sayfa sayfa görüntüle
less dosya.txt

# İlk satırları görüntüle
head dosya.txt

# Son satırları görüntüle
tail dosya.txt

# Dosya içinde arama
grep "aranan" dosya.txt

```

---

## 8. Log İnceleme

```bash

# Sistem loglarını izle
sudo journalctl -f

# Servis loglarını izle
sudo journalctl -u servisadi -f

```

---

## 9. Arşiv ve Sıkıştırma

```bash

# Klasörü .tar.gz formatında arşivle
tar -czvf arsiv.tar.gz klasor_adi

# Arşivi çıkar
tar -xzvf arsiv.tar.gz

```

---

## 10. Yetkilendirme ve İzinler

```bash

# İzinleri görüntüle
ls -l

# İzin değiştirme
chmod 755 dosya.txt   # rwxr-xr-x
chmod 644 dosya.txt   # rw-r--r--

# Sahip değiştirme
sudo chown kullanici:grup dosya.txt

```
