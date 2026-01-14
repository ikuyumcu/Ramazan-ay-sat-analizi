# Ramazan-ay-sat-analizi
🌙 Ramazan Ayı ve Bayram Satış Analizi Projesi (2022-2025)
Bu proje, 2022-2025 yılları arasındaki 4 yıllık satış verilerini (Koli ve TL bazında) inceleyerek, Ramazan ayının ve Ramazan Bayramı öncesindeki 4 günlük kritik dönemin satış performansını analiz eder. Proje, geçmiş verilerden öğrenen bir model ile 2025 yılı projeksiyonu oluşturmayı ve gerçekleşen verilerle bu projeksiyonu kıyaslamayı amaçlar.

🎯 Projenin Amacı ve İş Değeri
Bu analiz sadece rakamsal değişimleri değil, aşağıdaki stratejik soruları yanıtlamayı hedefler:

Operasyonel Planlama: Bayram öncesi son 4 günde yaşanan satış patlaması, lojistik ve depo kapasitesini ne kadar zorluyor? 




Mevsimsel Trend Analizi: Ramazan ayı satışlarda bir durgunluk mu yoksa bir fırsat dönemi mi yaratıyor? 




Hacim vs. Değer Dengesi: Büyüme gerçek bir talep artışından mı (Koli) yoksa fiyat artışlarından mı (TL) kaynaklanıyor? 




Tahminleme: Geçmiş 3 yılın verileriyle bir sonraki yılın stok gereksinimi ne kadar isabetli öngörülebilir?

📊 Temel Analiz Bulguları (Özet)
Tarihsel Trend: 2022-2024 yılları arasında Ramazan ayı, bir önceki aya göre ortalama %-3.79 (Koli bazında) daralma göstermiştir. 



2025 Kırılımı: 2025 yılında bu trend kırılarak Ramazan ayında %+6.06 büyüme kaydedilmiştir. 

Bayram Yoğunluğu: Bayramdan önceki son 4 günün günlük satış hızı, normal Ramazan günlerine göre ortalama %+33.69 daha yüksektir. 

🛠 Teknik Detaylar ve Metodoloji
Analiz sürecinde veri setinin yapısına (nokta azlığına) en uygun olan İstatistiksel Oransal Analiz yöntemi seçilmiştir.

Kullanılan Araçlar

Python 3.10+: Ana geliştirme dili.

Pandas: Veri manipülasyonu, birim ayrıştırma (Koli/TL) ve tablo oluşturma.

NumPy: Normalizasyon ve varyans hesaplamaları.

Uygulanan Analitik Yöntemler

Veri Normalizasyonu (Velocity Analysis): 30 günlük aylar ile 4 günlük özel günler, "Günlük Satış Hızı" metriğine indirgenerek kıyaslanabilir hale getirilmiştir.

Tarihsel Projeksiyon: 2022-2024 yıllarının mevsimsel katsayıları (Ratio 
Ram/Oncesi
​	
 , Ratio 
Bayram/Ram
​	
 ) hesaplanarak 2025 yılı başlangıç verisine uygulanmıştır.

Varyans (Sapma) Analizi: Tahmin edilen (Predicted) değerler ile gerçekleşen (Actual) veriler karşılaştırılarak modelin başarısı ölçülmüştür. (Koli bazlı tahmin hata payı: %9.29).

📈 Analiz Metrikleri (KPIs)
Ramazan Değişimi: ((Ramazan−Oncesi)/Oncesi)∗100 

Bayram Hızı Artışı: ((Bayram_4_Gun / 4) / (Ramazan / 30) - 1) * 100 

Birim Başı Gelir: TL bazlı büyümenin Koli bazlı büyümeyle korelasyonu. 

📁 Proje Yapısı
/data: Ham satış verileri (Koli ve TL).

/src: tahmin_modeli.py (Analiz ve tahmin algoritması).

/reports: yillik_satis_analizi.csv (Otomatik üretilen sonuç tablosu).

🚀 Sonuç
Analiz, 2025 yılının geçmiş yıllardan farklı bir büyüme ivmesine sahip olduğunu ve bayram öncesi dönemlerin operasyonel olarak en kritik (peak) noktalar olduğunu matematiksel olarak kanıtlamaktadır.
