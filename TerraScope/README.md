# 🌍 TerraScope — Çok Boyutlu Kentsel Dirençlilik ve İklim Simülasyonu

> 🚧 **Not:** Bu portföy şu anda güncelleme aşamasındadır. Ekran görüntüleri ve demo görselleri yakında eklenecektir. Kaynak kod özel tutulmakta olup talep üzerine veya görüşme sürecinde paylaşılabilir.

> Türkiye genelini ve İstanbul'un tüm ilçelerini kapsayan, canlı verilerle çalışan interaktif bir kentsel dirençlilik ve iklim riski simülasyon platformu.
> *Üniversite Bitirme Projesi — Haziran 2026*

---

## 📌 Özet

TerraScope; şehirlerin iklim ve afet risklerini çok boyutlu olarak değerlendiren, canlı ve statik verileri harmanlayarak geleceğe yönelik projeksiyonlar üreten interaktif bir karar destek platformudur. Türkiye'deki 81 ili ve İstanbul'un tüm ilçelerini (Adalar'dan Zeytinburnu'na) detaylı kırılımlarla kapsar.

## ✨ Öne Çıkan Özellikler

- **Canlı + statik veri füzyonu:** Open-Meteo REST API'siyle anlık hava kalitesi (AQI) ve meteoroloji verilerini; topografya, su endeksi ve deprem riski gibi statik verilerle birleştiren modüler bir veri motoru (CityDataEngine).
- **Geleceğe projeksiyon:** Demografik baskı ve küresel sanayi ivmesi parametrelerine göre 2026–2050 arası projeksiyon yapan, finansal eko-hasar ve "Dirençlilik Skoru" hesaplayan bir karar motoru (UrbanDecisionEngine).
- **İnteraktif görselleştirme:** Streamlit ve Folium ile kurumsal/karanlık temalı arayüz; riskli bölgeler için dinamik ısı haritaları (HeatMap).
- **Eylem planı üretimi:** Algoritmaya dayalı, bakanlık seviyesinde kentsel eylem önerileri (örn. Sünger Şehir, Biyo-hendek).

## ⚙️ Nasıl Çalışıyor?

1. Statik ve dinamik (canlı API) veri kaynakları toplanır ve ön işlemeden geçirilir.
2. CityDataEngine bu verileri il/ilçe bazında birleştirip yapılandırır.
3. UrbanDecisionEngine, seçilen parametrelere göre projeksiyon yapar ve Dirençlilik Skoru'nu hesaplar.
4. Sonuçlar Streamlit arayüzünde dinamik ısı haritaları ve eylem önerileriyle görselleştirilir.

## 🛠️ Kullanılan Teknolojiler

`Python` · `Streamlit` · `Folium` · `Pandas` · `NumPy` · `REST API (Open-Meteo)`

## 📷 Ekran Görüntüleri & Demo

> 🚧 _Yakında eklenecek — arayüz görüntüleri, ısı haritası örnekleri ve kısa bir demo._

---

🔒 *Kaynak kod özel tutulmaktadır; talep üzerine veya görüşme sürecinde paylaşılabilir.*
