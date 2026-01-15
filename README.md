# Ramazan-ay-sat-analizi
# 🌙 Ramazan Ayı ve Bayram Satış Analizi (2022 - 2025)

Bu proje, 2022 ile 2025 yılları arasındaki **Ramazan ayı öncesi, Ramazan ayı, Bayram dönemi (son 4 gün) ve Ramazan sonrası** satış verilerini analiz etmek amacıyla geliştirilmiştir. Analiz hem **Koli (Adet)** hem de **TL (Ciro)** bazında yapılarak, dönemsel talep değişimleri ve bayram satış hızı artışları incelenmiştir.

## 📊 Analiz Kapsamı ve Metodoloji

Projenin temel odak noktası, Ramazan ayındaki genel durağanlığın, bayram öncesi yoğunluğu ile nasıl ayrıştığını matematiksel olarak ortaya koymaktır. Bu kapsamda aşağıdaki temel performans göstergeleri (KPI) hesaplanmıştır:

* **Ramazan Etkisi:** Ramazan ayındaki satışların, bir önceki ve bir sonraki aya göre yüzde (%) değişimi.
* **Bayram Payı:** Ramazan ayının son 4 günündeki (Bayram dönemi) satışların toplam Ramazan ayı içindeki payı.
* **Bayram Satış Hızı Artışı:** Bayramdaki 4 günlük **günlük satış ortalamasının**, Ramazan ayının geneline göre ne kadar hızlandığını ölçen özel formül:

$$\text{Hız Artışı} = \left( \frac{\text{Bayram Satışı} / 4}{\text{Ramazan Satışı} / 30} - 1 \right) \times 100$$

## 🎯 Projenin Amacı ve Tahminleme Yaklaşımı

Bu çalışma, sadece geçmiş veriyi raporlamakla kalmayıp, ileriye dönük bir tahminleme disiplini oluşturmayı amaçlamaktadır:

1.  **Tahmin ve Doğrulama:** 2022, 2023 ve 2024 yılları verileri kullanılarak 2025 projeksiyonu oluşturulmaya çalışılmıştır. Ancak mevsimsel kaymalar ve pazar dinamikleri nedeniyle oluşan **hata payları** analiz edilmiştir. Gerçekleşen 2025 verileri ile tahminler karşılaştırılarak modelin tutarlılığı test edilmiştir.
2.  **Sürekli İyileştirme:** Yapılan bu sağlamaların temel amacı, geçmişteki sapmaları anlayarak **2026 yılı için çok daha isabetli bir tahminleme modeli** geliştirmektir.
3.  **Ticari Farkındalık:** Proje, bayram, kampanya ve tatil gibi özel dönemlerin ticaret döngüsü içerisinde nasıl "gözle görülür" farklar yarattığını ve bu dönemlerin stratejik planlamadaki kritik önemini ortaya koymaktadır.

## 📈 Öne Çıkan Bulgular

* **Mevsimsel Dalgalanma:** Satışların Ramazan ayında belirli bir trend izlediği, ancak 2025 verilerinde önceki yıllara göre farklı dinamiklerin (mevsimsel farklar) devreye girdiği gözlemlenmiştir.
* **Bayram Patlaması:** Bayramın son 4 gününde, günlük satış hızının normal Ramazan günlerine göre ciddi bir artış (bazı yıllarda %30+) gösterdiği tespit edilmiştir.
* **Ciro vs Adet:** TL bazındaki büyümenin, enflasyonist etkiler nedeniyle Koli bazındaki büyümeden daha dik bir eğime sahip olduğu doğrulanmıştır.

## 🛠️ Kullanılan Teknolojiler

* **Python 3.x**
* **Pandas:** Veri manipülasyonu ve analizi.
* **Matplotlib & Seaborn:** İstatistiksel veri görselleştirme.
* **Google Colab:** Geliştirme ortamı.

---
*Bu analiz İbrahim Kuyumcu tarafından veri odaklı karar alma süreçlerini iyileştirmek amacıyla hazırlanmıştır.*
