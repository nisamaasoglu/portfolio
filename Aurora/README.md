# 🎨 Aurora — Gerçek Zamanlı, Sesle Yönlendirilen Üretken Sanat Motoru

> 🚧 **Not:** Bu portföy şu anda güncelleme aşamasındadır. Ekran görüntüleri ve demo görselleri yakında eklenecektir. Kaynak kod özel tutulmakta olup talep üzerine veya görüşme sürecinde paylaşılabilir.

> Canlı ses verisini analiz edip, sesin duygusuna göre şekillenen dinamik dijital sanata dönüştüren sıfır gecikmeli bir üretken sistem.
> *Ocak 2026*

---

## 📌 Özet

Aurora, mikrofondan gelen canlı sesi gerçek zamanlı analiz eder; sesin frekans ve nota özelliklerinden "duygu" çıkarımı yapar ve bu veriyi web arayüzünde dinamik, üretken görsellere dönüştürür. İnsan sesindeki mikroskobik duygu değişimlerini yakalayıp dijital sanata çevirmeyi amaçlar.

## ✨ Öne Çıkan Özellikler

- **Gerçek zamanlı ses analizi:** Librosa ve NumPy ile canlı mikrofon verisi 44.1 kHz'de işlenir; RMS (ses şiddeti), Spectral Centroid (parlaklık), Rolloff ve Chroma (nota) metrikleri çıkarılır (EmotionAnalyzer).
- **Duygu eşleme:** Frekans ve nota verilerini matematiksel eşiklerle 6 temel duyguya (sakin, mutlu, heyecanlı, üzgün, kızgın, nötr) eşleyen özel karar algoritması.
- **Sıfır gecikmeli iletişim:** AIOHTTP ile kurulan asenkron WebSocket sunucusu, duygu ve perde (pitch) verisini web arayüzüne JSON olarak anlık aktarır.
- **Üretken sanat altyapısı:** Analiz çıktısını frontend'de eşsiz, dinamik görsel eserlere çeviren bir altyapı.

## ⚙️ Nasıl Çalışıyor?

1. Mikrofon girişi gerçek zamanlı yakalanır.
2. Librosa/NumPy ile frekans-yoğunluk metrikleri (RMS, Spectral Centroid, Rolloff, Chroma) çıkarılır.
3. Karar algoritması bu metrikleri 6 temel duygudan birine eşler.
4. Sonuç, AIOHTTP WebSocket sunucusu üzerinden web arayüzüne sıfır gecikmeyle aktarılıp görsele dönüştürülür.

## 🛠️ Kullanılan Teknolojiler

`Python` · `Librosa` · `NumPy` · `PyAudio` · `Asyncio` · `WebSockets (AIOHTTP)`

## 📷 Ekran Görüntüleri & Demo

> 🚧 _Bu proje görselle en çok parlayan projen — yakında kısa bir ekran kaydı (GIF/video) eklenecek._

---

🔒 *Kaynak kod özel tutulmaktadır; talep üzerine veya görüşme sürecinde paylaşılabilir.*
