# Ubuntu Paket Yönetimi (APT) ve Git Kurulumu

Ubuntu’da paket yönetimi **APT** (Advanced Package Tool) üzerinden yapılır.  
APT, yazılım paketlerini indirme, kurma, güncelleme ve kaldırma işlemlerini yönetir.

---

## 1. Paket Listesini Güncelleme
Yeni bir paket kurmadan önce paket listelerini güncellemek iyi bir alışkanlıktır.

```bash
sudo apt update
```

Bu komut, sistemdeki paketlerin en güncel versiyon bilgilerini çeker.


## 2. Mevcut Paketleri Güncelleme

Kurulu tüm paketleri en son sürüme yükseltir.


```bash
sudo apt upgrade -y
```

-y parametresi tüm onayları otomatik verir.



## 3. Belirli Bir Paketi Kurma

Format:
```bash
sudo apt install paket-adi
```

Örnek:
```bash
sudo apt install curl
```


## 4. Paketi Kaldırma
Format:
```bash
sudo apt remove paket-adi
```

Örnek:
```bash
sudo apt remove curl
```

Tamamen silmek için (ayar dosyaları dahil):
```bash
sudo apt purge paket-adi
```


## 5. Paket Arama

Format:
```bash
apt search kelime
```

Örnek:
```bash
apt search nginx
```

## 6. Paket Hakkında Bilgi

Format:
```bash
apt show paket-adi
```

Örnek:
```bash
apt show git
```

## 7. Önbellek Temizleme
APT indirilen paketleri /var/cache/apt/archives dizininde saklar. Temizlemek için:
```bash
sudo apt clean
sudo apt autoclean
```

Kullanılmayan bağımlılıkları silmek için:
```bash
sudo apt autoremove
```

## 8. Örnek: Git Kurulumu
Git, versiyon kontrol sistemi olarak yazılım geliştirmede çok önemlidir.
Ubuntu’ya Git yüklemek için:
```bash
# Paket listelerini güncelle
sudo apt update

# Git’i yükle
sudo apt install git -y

# Kurulum doğrulama
git --version

```

Beklenen çıktı (örnek):
```bash
git version 2.43.0
```

## 9. Git İlk Yapılandırma
Kurulum sonrası Git’e kullanıcı adınızı ve e-posta adresinizi tanımlayın:
```bash
git config --global user.name "DevrimMehmet"
git config --global user.email "devrimmehmet@gmail.com"
```

Ayarları kontrol etmek için:
```bash
git config --list
```
