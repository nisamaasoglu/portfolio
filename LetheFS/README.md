# 🗂️ LetheFS — Ebbinghaus Tabanlı Akıllı Dosya Arşivleyici

> 🚧 **Not:** Bu portföy şu anda güncelleme aşamasındadır. Ekran görüntüleri ve demo görselleri yakında eklenecektir. Kaynak kod özel tutulmakta olup talep üzerine veya görüşme sürecinde paylaşılabilir.

> İnsan belleğinin unutma eğrisinden ilham alan, dosyaları otonom önceliklendirip güvenle arşivleyen, tamamen offline çalışan bir masaüstü asistanı.
> *Nisan 2026*

---

## 📌 Özet

LetheFS, Hermann Ebbinghaus'un matematiksel **unutma eğrisi** modelini yazılıma taşır: az kullanılan dosyalar zamanla "unutulur" ve güvenle arşivlenir, kritik dosyalar korunur. İnternete ihtiyaç duymadan, %100 yerel çalışarak tam veri gizliliği sağlar.

## ✨ Öne Çıkan Özellikler

- **Unutma eğrisi algoritması:** Dosyaların kullanım sıklığı ve son erişimine göre dinamik bir "unutulmuşluk skoru" hesaplayan aralıklı tekrar (spaced-repetition) mantığı.
- **Gerçek zamanlı izleme:** Watchdog ile işletim sistemi seviyesinde sessiz çalışan bir arka plan motoru (daemon); veriler anlık olarak SQLite'a işlenir.
- **Hata toleransı & geri alma:** "Asla silme, güvenle arşivle" prensibi; isim çakışmalarını çözer, tüm işlemleri JSONL log'a yazarak tek tıkla geri alma sağlar.
- **Akıllı yönetim:** Dosya türüne göre ağırlıklandırma (ör. .docx ↔ .png), beyaz liste (whitelist) yönetimi ve Windows görev zamanlayıcı entegrasyonu.
- **Arayüz:** Hem masaüstü uygulaması hem komut satırı arayüzü (CLI).

## ⚙️ Nasıl Çalışıyor?

1. Watchdog daemon'ı dosya erişimlerini gerçek zamanlı dinler ve SQLite'a kaydeder.
2. Skorlama algoritması her dosyaya kullanım sıklığı + son erişime göre bir "unutulmuşluk skoru" atar.
3. Belirlenen eşik aşıldığında düşük skorlu dosyalar güvenle arşivlenir; beyaz listedekiler korunur.
4. Tüm taşıma işlemleri JSONL log'a yazılır, böylece tek tıkla geri alınabilir.

## 🛠️ Kullanılan Teknolojiler

`Python 3.10+` · `SQLite` · `Watchdog` · `JSONL`

## 📷 Ekran Görüntüleri & Demo

> 🚧 _Yakında eklenecek — CLI ve masaüstü arayüzünden görüntüler._

---

🔒 *Kaynak kod özel tutulmaktadır; talep üzerine veya görüşme sürecinde paylaşılabilir.*
