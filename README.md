# 🎨 Runeterra Manzaraları: Bir Web Galerisi

League of Legends dünyasından estetik kesitleri gösteren modern ve responsive bir web galerisi uygulaması.


https://veyse1.github.io/Resim-Galerisi--devi/
---


## 📋 İçindekiler

- [Proje Hakkında](#proje-hakkında)
- [Dosya Yapısı](#dosya-yapısı)
- [Özellikler](#özellikler)
- [Teknolojiler](#teknolojiler)
- [Kurulum](#kurulum)
- [Kullanım](#kullanım)
- [Responsive Tasarım](#responsive-tasarım)
- [Modal Sistemi](#modal-sistemi)
- [Telif Hakkı](#telif-hakkı)

---

## 🎯 Proje Hakkında

Bu proje, **eğitim amaçlı** olarak geliştirilmiş modern bir resim galerisi uygulamasıdır. League of Legends oyunundaki Runeterra dünyasından 35 adet estetik kesiti içerir ve 4 kategoride sunur:

- **Freljord** - Dondurucu diyarın mahzenli yapıları
- **Bilgewater** - Denizin kaotik limanları
- **Ionia** - Doğanın ruhani güzelliği
- **Shurima/Noxus/Piltover** - İmparatorlukların görkemi

---

## 📁 Dosya Yapısı

```
Resim Galerisi V2/
├── index.html              # Ana HTML dosyası (Modal sistemi + JavaScript)
├── style.css              # Tüm CSS stilleri
├── README.md              # Bu dosya
└── resimler/              # 35 adet resim klasörü
    ├── Ayazboynuz Zirvesi'nin altındaki Buzdoğan Mahzenleri.jpg
    ├── BILGEWATER KÖRFEZİ.jpg
    ├── BUHRU TAPINAĞI.jpg
    ├── ... (32 adet daha)
    └── ŞARKI VADİSİ.jpg
```

---

## ✨ Özellikler

### 🖼️ Galeri İşlevselliği
- **35 Resim** - Tüm League of Legends bölgelerinden kesitler
- **Dinamik Yapı** - JavaScript ile jQuery'siz olarak dinamik kart oluşturma
- **Sadece Başlıklar** - Kartlarda sadece başlık görünüyor
- **Resim Kalitesi Korunuyor** - `object-fit: cover` ile kesintisiz görüntü

### 🎯 Modal Açılır Pencere
- **Tıkla ve Aç** - Herhangi bir karta tıklayarak modal açılır
- **Orijinal Boyut** - Resim modal'da orijinal boyutunda gösterilir
- **Açıklama Metni** - Her resmin detaylı açıklaması gösterilir
- **Kapatma Seçenekleri**:
  - ❌ X butonuna tıkla
  - 🔙 Modal arka planına tıkla
  - ⌨️ ESC tuşu

### 📱 Responsive Tasarım
- **Masaüstü** (1024px+) - 3-4 sütunlu grid
- **Tablet** (768px-1024px) - 2 sütunlu grid
- **Mobil** (640px ve altı) - 1 sütunlu grid
- **Büyük Kart** - İlk kart 2x2 grid kaplar (masaüstü'nde)

### 🎨 Tasarım Özellikleri
- **Koyu Tema** - #1a1d22 arka planı
- **Glassmorphism** - Blur efektli transparent kartlar
- **Smooth Animasyonlar** - Kart hover ve modal açılış animasyonları
- **Şık Typography** - Montserrat ve Inter fontları

### ⚡ Performans
- **Hafif** - jQuery veya başka kütüphane yok
- **Hızlı Yükleme** - Resimler lazy loading desteği
- **İyi SEO** - Semantic HTML struktur
- **Accessibility** - ALT metinler tüm resimlerde

---

## 🛠️ Teknolojiler

| Teknoloji | Versiyon | Kullanım |
|-----------|----------|----------|
| HTML5 | - | Yapı ve semantik |
| CSS3 | - | Stil ve animasyonlar |
| JavaScript (Vanilla) | ES6+ | Dinamik işlevsellik |
| Grid/Flexbox | - | Layout sistemi |

**Kütüphane Yok** ✓ - Tamamen vanilla JavaScript kullanıyor

---

## 🚀 Kurulum

### Gereksinimler
- Herhangi bir web tarayıcı (Chrome, Firefox, Safari, Edge)
- Dosya sistemi erişimi
- İnternet bağlantısı (isteğe bağlı - yerel olarak çalıştırılabilir)

### Adımlar
1. Dosyaları bir klasöre yerleştir
2. `index.html` dosyasını tarayıcıda aç (Çift tık yeterli)
3. Veya yerel sunucu ile çalıştır:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # Node.js (http-server kullanan)
   npx http-server
   ```

---

## 📖 Kullanım

### Galeriye Bakmak
1. Sayfa açıldığında otomatik olarak tüm kartlar görünür
2. İstediğin resmin başlığını oku
3. Karta tıkla → Modal açılır

### Modalı Kullanmak
1. **Resmi Görüntüle** - Orijinal çözünürlükte her detayı gör
2. **Açıklamasını Oku** - Resmin altında dolu bir metin bulabilirsin
3. **Kapatmak** için:
   - X'e tıkla
   - ESC tuşuna bas
   - Arka alana tıkla

### Farklı Cihazlarda Test Et
- 📱 Telefon (640px)
- 📱 Tablet (768px)
- 💻 Masaüstü (1024px+)

---

## 📱 Responsive Tasarım

### Masaüstü (1024px+)
```
┌──────────────┬──────────────┬──────────────┐
│     KART     │     KART     │     KART     │
├──────────────┼──────────────┼──────────────┤
│   BYKK KART  │   BYKK KART  │     KART     │
│   (2x2)      │   (2x2)      │              │
├──────────────┴──────────────┼──────────────┤
│     KART     │     KART     │     KART     │
└──────────────┴──────────────┴──────────────┘
```

### Tablet (768px-1024px)
```
┌──────────────┬──────────────┐
│     KART     │     KART     │
├──────────────┼──────────────┤
│     KART     │     KART     │
└──────────────┴──────────────┘
```

### Mobil (640px ve altı)
```
┌──────────────┐
│     KART     │
├──────────────┤
│     KART     │
├──────────────┤
│     KART     │
└──────────────┘
```

---

## 🎯 Modal Sistemi

### Nasıl Çalışır
1. **Tıklama Olayı** - Karta tıklandığında `openModal(item)` fonksiyonu çalışır
2. **Veri Yükleme** - Seçilen resmin title, description ve image URL'i modal'a eklenir
3. **Modal Açılış** - CSS animasyonu ile fade-in ve slide-in efektleri
4. **Kapatma** - Kullanıcı X, ESC veya arka alana tıkladığında modal kapanır

### JavaScript Fonksiyonları
```javascript
// Modal aç
openModal(item) {}

// Modal kapat
closeModal() {}

// Arka alana tıkla ile kapatma
closeModalOnBg(event) {}

// ESC tuşu ile kapatma
document.addEventListener('keydown', (e) => {})

// Galeriyi başlat
initGallery() {}
```

---

## 🎨 Tasarım Detayları

### Renkler
- **Arka Plan** - `#1a1d22` (Koyu gri)
- **Kart Arka Plan** - `rgba(232, 220, 200, 0.08)` (Light transparent)
- **Metin Rengi** - `#e8e8e8` (Açık beyaz)
- **İkincil Metin** - `#c9c9c9` (Açık gri)

### Fontlar
- **Başlıklar** - Montserrat (Bold)
- **Açıklamalar** - Inter (Regular)
- **Fallback** - Segoe UI, Tahoma, Geneva, Verdana

### Animasyonlar
- **Kart Hover** - Y ekseni -8px, shadow artırma
- **Modal Açılış** - Fade-in (0.3s) + Slide-in (0.3s)
- **Modal Kapanış** - Fade-out (0.3s)

---

## 🔧 Özel CSS Özellikleri

### object-fit: cover
Resimler kartı doldurur ama oranını korur, kırpılmaz

### backdrop-filter: blur(10px)
Kartlarda ve modalde glassmorphism efekti

### grid-auto-fit
Responsive grid otomatik ayarlanır

### box-shadow (inset)
Kartlarda iç gölge efekti

---

## 📊 İstatistikler

| Metrik | Değer |
|--------|-------|
| Toplam Resim | 35 |
| Resim Kategorisi | 5 (Freljord, Bilgewater, Ionia, Shurima/Noxus, Piltover) |
| JavaScript Satır | ~280 |
| CSS Satır | ~200 |
| HTML Satır | ~50 (dinamik HTML) |
| Dosya Boyutu | ~50KB (HTML+CSS, resimler hariç) |
| Responsive Breakpoint | 3 (1024px, 768px, 640px) |

---

## 🐛 Bilinen Sınırlamalar

1. **Modern Tarayıcı Gerekli** - CSS Grid ve Flexbox desteği zorunlu
2. **Resim Boyutu** - Büyük JPG dosyaları yavaş yükleme yapabilir
3. **İnternet Dosyaları** - Yerel olmayan fontlar yükleme gerektirir
4. **Mobil Safari** - Bazı CSS efektleri sınırlı olabilir

---

## 🚀 Geliştirme İdeaları

- [ ] Resim görselleri optimize et (WebP format)
- [ ] Infinite scroll özelliği ekle
- [ ] Filtreleme seçeneği ekle (kategoriye göre)
- [ ] Arama fonksiyonu ekle
- [ ] Favorilere ekleme özelliği
- [ ] PDF indirme seçeneği
- [ ] Sosyal medya paylaşımı
- [ ] Karanlık/Aydınlık tema seçeneği
- [ ] Resim slider/kaydırma sağ-sol
- [ ] Right-click koruma

---

## 📝 Telif Hakkı

⚠️ **Bu proje eğitim amaçlı hazırlanmıştır.**

Kullanılan görsellerin tüm hakları **Riot Games**'e aittir. Bu proje Riot Games'in fikri mülkiyet politikasına uygun olarak hazırlanmıştır.

```
© 2026 Eğitim Projesi
© Riot Games - Tüm görseller
```

---

## 📧 İletişim ve Katkılar

Bu proje eğitim amaçlı bir öğrenci projesidir. Katkılar ve öneriler memnuniyetle karşılanır!

---

## 📚 Kaynaklar

- [League of Legends Official](https://www.leagueoflegends.com/)
- [Riot Games Rights](https://www.riotgames.com/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS Tricks](https://css-tricks.com/)

---

**Son Güncelleme:** 11 Nisan 2026
**Versiyon:** 1.0
**Durum:** ✅ Tamamlandı