# 📸 Responsive Resim Galerisi - Ödev 6

Çağdaş web teknolojileri kullanılarak oluşturulmuş, tam uyumlu (responsive) ve modern tasarıma sahip bir resim galerisi uygulaması.

---

## 🔗 Site Linki

https://veyse1.github.io/Web-Project-6/

---

---

## 🌟 Özellikler

✅ **Tam Responsive Tasarım**
- Desktop (1024px+)
- Tablet (768px - 1024px)
- Mobile (640px ve altı)
- Extra Small (480px ve altı)

✅ **Modern CSS Grid Layout**
- `repeat()` - Dinamik sütun tekrarı
- `gap` - Aralar arası boşluk kontrolü
- `minmax()` - Esnek boyutlandırma
- `auto-fit` - Otomatik sıra sarması

✅ **İnteraktif Öğeler**
- Hover efektleri (ölçek, kaydırma, gölge)
- Resim parlaklık ve doygunluk değişimleri
- Smooth geçişler ve animasyonlar
- Featured badge ve özel simgeler

✅ **Profesyonel Tasarım**
- Koyu tema (Dark Mode)
- Gradient metin ve görseller
- Mor-mavi renk paleti (#BB86FC, #9C7FD9)
- Özel TypeScript benzeri font ailesi

✅ **47 Adet Resim Kartı**
- 1 büyük kart (featured) - 2×2 grid span
- 2 özel içerikli kart (badge ve animasyon)
- 44 standart kart
- Picsum.photos'tan yüksek kaliteli görseller

---

## 🛠️ Teknolojiler

| Teknoloji | Kullanım |
|-----------|----------|
| **HTML5** | Semantik yapı ve DOCTYPE |
| **CSS3** | Grid, Flexbox, Media Queries, Animasyonlar |
| **JavaScript** | Opsiyonel (şu anda saf CSS/HTML) |
| **Picsum.photos** | Dinamik resim kaynağı |

---

## 📁 Dosya Yapısı

```
Web Ödev 6/
├── index.html          # Ana HTML dosyası (47 kart + yapı)
├── styles.css          # Tüm CSS stillemeleri
├── README.md           # Bu dosya
└── (resimler picsum.photos'tan yükleniyor)
```


### Tarayıcı Uyumluluğu
- ✅ Chrome/Chromium (v90+)
- ✅ Firefox (v88+)
- ✅ Safari (v14+)
- ✅ Edge (v90+)

---

## 🎨 Renk Paleti

| Renk | Kod | Kullanım |
|------|-----|----------|
| Arka Plan | `#121212` | Sayfa arka planı |
| Kart | `#1E1E1E` | Kart arka planı |
| Metin | `#E0E0E0` | Ana metin rengi |
| Vurgu | `#BB86FC` | Hover, linkler, gradientler |
| Ikincil Vurgu | `#9C7FD9` | Gradient efektleri |

---

## 📐 Grid Yapısı

### Desktop (1024px+)
```
[Large 500×400]  [Card 300×250]  [Card 300×250]
[Card 300×250]   [Card 300×250]  [Card 300×250]
```

### Tablet (768px - 1024px)
```
[Large 500×400]  [Card 300×250]
[Card 300×250]   [Card 300×250]
```

### Mobile (≤640px)
```
[Card 300×250]
[Card 300×250]
[Large 300×250]
```

---

## 🎬 Hover Efektleri

1. **Kart Animasyonu**
   - Yukarı kaydırma: `-10px`
   - Ölçek: `1.02x`
   - Gölge artışı ve gradient glow

2. **Resim Efektleri**
   - Parlaklık: `1.15`
   - Doygunluk: `1.3`

3. **Özel Kartlar**
   - Featured: Gradient overlay + badge
   - Special: Floating emoji animasyonu

---

## 📱 Responsive Breakpoints

| Breakpoint | Ekran Boyutu | Grid Sütunları |
|-----------|--------------|----------------|
| Desktop | ≥1024px | repeat(auto-fit, minmax(280px, 1fr)) |
| Tablet | 768px-1024px | repeat(auto-fit, minmax(240px, 1fr)) |
| Mobile | 640px ve altı | repeat(auto-fit, minmax(200px, 1fr)) |
| Extra Small | 480px ve altı | 1fr (tek sütun) |



## 📝 Notlar

- Tüm resimler **Picsum.photos** API'sinden yüklenir
- Sabit `random` parametreleri sayesinde her zaman aynı resimler görüntülenir
- CSS media queries ile tam responsive tasarım sağlanır
- No JavaScript required - saf HTML ve CSS

---

## ✏️ Ödev Detayları

**Ödev:** Web Tasarımı - Responsive Resim Galerisi   
**Teknoloji Gereksinimleri:**
- ✅ CSS Grid (repeat, gap, minmax, auto-fit)
- ✅ 6+ resim kartı (47 kart)
- ✅ 1 büyük kartı (featured card)
- ✅ Hover efektleri
- ✅ Responsive tasarım

---


---

**Son Güncelleme:** April 10, 2026  
**Sürüm:** 1.0
