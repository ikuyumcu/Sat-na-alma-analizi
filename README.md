Bu proje, bir içecek distribütörünün 4 yıllık (2022-2025) tarihsel satış verilerini kullanarak, Makine Öğrenmesi (Machine Learning) yöntemleriyle 2026 yılı için aylık satın alma stratejileri geliştirmek amacıyla oluşturulmuştur.

Geleneksel "sezgisel" satın alma yöntemlerini, Meta'nın Prophet kütüphanesi ve veri analitiği araçlarıyla modernize ederek stok maliyetlerini optimize etmeyi hedeflemektedir.

Proje Amacı
Ticari işletmelerde yanlış satın alma kararları ya gereksiz stok maliyetine (overstock) ya da talebin karşılanamamasına (out-of-stock) yol açar. Bu proje;

Geçmiş verideki gizli trendleri ortaya çıkarmak,

Ürün bazlı mevsimsellik etkilerini (yaz/kış talebi) hesaplamak,

2026 yılı için her ay bazında "ne kadar satın alınmalı?" sorusuna yanıt vermek için geliştirilmiştir.

Kullanılan Yöntemler ve Teknolojiler
Proje kapsamında uçtan uca şu veri bilimi adımları uygulanmıştır:

Veri Manipülasyonu & Temizleme: 40+ Excel tablosu Pandas ve NumPy kullanılarak kronolojik bir zaman serisine (Time Series) dönüştürüldü.

Zaman Serisi Modelleme (Meta Prophet): Satış tahminleri için Facebook (Meta) tarafından geliştirilen Prophet algoritması kullanıldı. Bu yöntemle:

Trend Analizi: Satışların yıllar içindeki genel büyüme ivmesi yakalandı.

Mevsimsellik (Seasonality): İçecek sektöründeki aylık ve mevsimsel dalgalanmalar (yazın artan vişne suyu talebi gibi) modellendi.

Güvenlik Payı (Safety Stock) Hesaplaması: Tahmin edilen rakamlara, tedarik zinciri risklerini (lojistik gecikmeler, ani talep artışları) yönetmek adına %5 operasyonel emniyet marjı eklendi.

Veri Görselleştirme: Matplotlib ve Seaborn ile 2025 gerçekleşen ve 2026 tahmini verileri kıyaslanarak görsel raporlar oluşturuldu.
