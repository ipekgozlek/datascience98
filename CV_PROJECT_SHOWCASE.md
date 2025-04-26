# Promosyon Satış Etkisi & Kanibalizasyon Analizi – Veri Bilimi Projesi

Bu proje, perakende sektöründe uygulanan promosyon kampanyalarının ürün satışlarına etkisini ölçmek ve benzer ürünler arasında oluşabilecek **kanibalizasyon** etkisini analiz etmek amacıyla gerçekleştirilmiştir.

---

## Proje Hedefleri
- Promosyon uygulanan ürünlerin satış artışını doğru bir şekilde tahmin etmek
- Aynı kategoride veya farklı kategorilerdeki ürünler arasında oluşabilecek kanibalizasyon etkisini tespit etmek
- Promosyon kampanyalarının genel satış performansına ve yatırım geri dönüşüne (ROI) olan etkisini analiz etmek

---

## Kullanılan Yöntem ve Teknikler
- **Veri Ön İşleme ve Feature Engineering**:
  - Satış geçmişi, ürün grupları, kampanya tarihleri gibi temel değişkenlerin hazırlanması
  - PrePromoAvg, ProductGroup1 ve ProductGroup2 değişkenlerinin Frequency Encoding yöntemiyle dönüştürülmesi
- **Modelleme**:
  - XGBoost regresyon modeli ile ürün bazlı satış tahmini
- **Kümeleme (Segmentation)**:
  - Mağazaların satış hızlarına göre (Fast / Medium / Slow) sınıflandırılması için K-Means algoritması kullanımı
- **Performans Değerlendirme**:
  - R²: 0.72
  - MAE: 0.12
  - Adjusted MAPE: 87%

---

## Öne Çıkan Bulgular
- Promosyon 5 kampanyası, hedef üründe %18 oranında satış artışı sağladı.
- Aynı ürün grubu içerisinde ve grup dışındaki ürünlerde satış düşüşleri tespit edilerek **hem within-group hem de cross-group cannibalization** etkileri belirlendi.
- Promosyon sonrası toplam kategori satışlarında %3 net artış gerçekleşti.
- Promosyonun yatırım geri dönüşü (ROI) hem net satışlar hem de promosyon sonrası geri dönüş hacimleri ile değerlendirildi.

---

## İleriye Yönelik Öneriler
- Model performansını artırmak ve iş etkisini daha iyi ölçmek için fiyat değişimleri, mağaza lokasyonu, mevsimsellik ve demografik faktörler gibi ek değişkenlerin dahil edilmesi önerildi.

---

## Teknik Sunum ve Değerlendirme
- 1 saatlik teknik mülakat oturumunda proje detayları sunuldu.
- Model mimarisi, değerlendirme metrikleri ve feature engineering süreçleri hakkında sorulara yanıt verildi.

---

##  Kullanılan Araçlar
- Python (Pandas, NumPy, Scikit-learn, XGBoost)
- Jupyter Notebook
- Excel (ön analizler için)

---

## 🔗 Projeye Git
[➡️ Tüm detayları görmek için buraya tıklayın](https://github.com/ipekgozlek/datascience98)

> Bu proje yalnızca özel inceleme amacıyla paylaşılmıştır.
