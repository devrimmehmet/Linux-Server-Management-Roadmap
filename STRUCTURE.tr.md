# Depo Yapısı ve İsimlendirme Standartları

## 1. Klasör İsimlendirme
- Ana bölümler için **PascalCase** kullanın (örn. `01-Basics`, `02-Docker`).
- Her ana bölüm şu alt klasörleri içermelidir:
  - `en/` klasörü → İngilizce içerikler
  - `tr/` klasörü → Türkçe içerikler
  - `media/` klasörü → İlgili görseller ve videolar

## 2. Dosya İsimlendirme
- Dosya isimlerinde **kebab-case** kullanın (örn. `docker-intro.md`, `ag-yonetimi.md`).
- `en/` klasöründeki dosya adları İngilizce, `tr/` klasöründeki dosya adları Türkçe olmalıdır.
- Dosya adlarında boşluk veya özel karakter kullanmayın.

## 3. Medya Dosyaları
- Bölüme ait tüm görsel ve videolar o bölümün `media/` klasöründe saklanmalıdır.
- Medya dosyalarında açıklayıcı ve kebab-case isimler kullanın (örn. `docker-architecture.png`).

## 4. Dil Dosyaları
- Ana README iki dilde olmalıdır:
  - `README.md` → İngilizce
  - `README.tr.md` → Türkçe
- Dosyaların en üst kısmında karşı dildeki versiyona yönlendiren bağlantı bulunmalıdır.

## 5. Versiyonlama
- Büyük içerik güncellemeleri net commit mesajları ile yapılmalıdır:
  - Örnek: `docs(en): added docker compose guide`
  - Örnek: `docs(tr): güncellendi kubernetes giriş notları`

## 6. Katkı Kuralları
- Yeni eklenen içerik mümkünse hem **İngilizce** hem **Türkçe** olarak eklenmelidir.
- Medya dosyaları web için optimize edilmiş olmalıdır (kalite kaybı olmadan sıkıştırılmış).

---
