# OLS Regresyon Analizörü

Bu proje, çoklu doğrusal regresyon analizini adım adım gösteren interaktif bir web uygulamasıdır. Uygulama, Ordinary Least Squares (OLS) yöntemi ile regresyon katsayılarını hesaplar ve tüm ara işlemleri detaylı şekilde sunar.

## Özellikler

- 📊 Detaylı regresyon analizi (13 bölüm)
- 📱 Tamamen responsive tasarım
- 🌙 Siyah tema arayüz
- 📈 Gerçek zamanlı hesaplama
- 📋 Türkçe arayüz
- 🧮 Adım adım hesaplama gösterimi

## Kurulum

### Gereksinimler
- Node.js (v14 veya üzeri)
- npm (Node.js ile birlikte gelir)

### Kurulum Adımları

1. Repoyu klonlayın:
```bash
git clone <repo-url>
cd ols-regression-analyzer
```

2. Bağımlılıkları yükleyin:
```bash
npm install
```

3. Geliştirme sunucusunu başlatın:
```bash
npm run dev
```

4. Tarayıcınızda `http://localhost:5173` adresine gidin

## Kullanım

1. Uygulama açıldığında veri giriş tablosu görünür
2. Y (bağımlı değişken) ve X1, X2 (bağımsız değişkenler) değerlerini tabloya girin
3. "Analiz Et" butonuna tıklayın
4. Detaylı regresyon analizi sonuçlarını görüntüleyin:
   - Veri özeti ve doğrulama
   - Detaylı veri tablosu (ortalamadan sapmalar)
   - Model tanımı ve katsayı hesaplamaları
   - En küçük kareler katsayı tahminleri
   - Tahmin edilen değerler ve artıklar
   - Kareler toplamı analizi
   - Regresyonun standart hatası
   - Katsayıların standart hataları
   - t-istatistikleri ve anlamlılık testleri
   - Genel model anlamlılığı (F-testi)
   - Ortalama ve nokta esnekliği
   - İstatistiksel ve iktisadi yorum
   - Tüm formüller - hızlı referans

## Teknolojiler

- **React** - Kullanıcı arayüzü
- **Vite** - Derleme aracı
- **JavaScript** - Hesaplama motoru
- **CSS** - Stil ve tasarım

## Geliştirme

### Kod Yapısı

```
src/
├── components/
│   └── OLSRegression.jsx    # Ana regresyon bileşeni
├── styles/
│   └── OLSRegression.css    # Stil dosyaları
├── utils/
│   └── olsCalculations.js   # Matematiksel hesaplamalar
├── App.jsx                  # Ana uygulama bileşeni
└── main.jsx                 # Uygulama giriş noktası
```

### Özel Hesaplama Özellikleri

- OLS katsayı tahminleri (matris formülü)
- Normal denklemler yöntemi (b₂ → b₁ → b₀ sırası)
- Ortalamadan sapma hesaplamaları
- Detaylı adım adım formül gösterimi
- Esneklik analizleri

## Lisans

Bu proje MIT Lisansı ile lisanslanmıştır. Detaylar için [LICENSE](LICENSE) dosyasına bakın.

## Katkı

Katkıda bulunmak için:
1. Forklayın
2. Yeni bir branch oluşturun (`git checkout -b feature/yeni-ozellik`)
3. Değişikliklerinizi commit edin (`git commit -am 'Yeni özellik ekle'`)
4. Branch'inizi push edin (`git push origin feature/yeni-ozellik`)
5. Pull request oluşturun