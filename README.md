# 💧 Su İçilebilirlik Analizi (Water Potability Analysis)

_Hazırlayan: Doğukan Sark_

📘 Proje Özeti

Bu proje, suyun içilebilirliğini (potability) belirlemek amacıyla çeşitli kimyasal ve fiziksel özelliklere dayalı bir uçtan uca veri bilimi çalışmasıdır.

Amaç, suyun pH değeri, sertliği, çözünmüş katı madde oranı, sülfat ve trihalometan düzeyleri gibi özelliklerin içilebilirlik üzerindeki etkisini analiz etmek ve bu verilerle suyun içilebilir olup olmadığını tahmin eden bir makine öğrenimi modeli geliştirmektir.

Proje, veri temizleme, görselleştirme, modelleme ve değerlendirme aşamalarının tümünü göstermektedir ve tamamen Google Colab uyumlu olarak hazırlanmıştır.

---

## 🚀 Öne Çıkan Özellikler ve Metodoloji

* 📊 Veri Keşfi (EDA): Seaborn, Matplotlib ve Plotly kullanılarak kapsamlı görselleştirmeler ile veri dağılımının ve değişkenler arası ilişkilerin incelenmesi.
* 🧹 Eksik Veri İşleme (Imputation): Eksik değerlerin (NaN) dağılımı Missingno kütüphanesi ile incelendikten sonra, medyan tabanlı doldurma (imputation) yöntemiyle yönetilmesi.
* 🧠 Gelişmiş Modelleme Süreci: Yaygın kullanılan Decision Tree ve Random Forest sınıflandırıcılarının karşılaştırılması.
* ⚙️ Model Optimizasyonu: Performans iyileştirmesi için RandomizedSearchCV ile hiperparametre optimizasyonu ve RepeatedStratifiedKFold ile tekrarlı çapraz doğrulama uygulanması.
* 📈 Model Değerlendirme: Sınıflandırma problemlerinde kritik olan Precision Score ve Confusion Matrix analizi.

---

## 🧰 Kullanılan Teknolojiler

| Kategori | Kütüphane / Araç |

| Programlama Dili | Python 3 |
| Veri İşleme | Pandas, NumPy |
| Görselleştirme | Matplotlib, Seaborn, Plotly, Missingno |
| Makine Öğrenimi | scikit-learn |
| Çalışma Ortamı | Google Colab (Tam Uyumluluk) |

---

📊 Görselleştirme ve Analiz Çıktıları

🔹 Su İçilebilirlik Dağılımı

Potable (1) ve Not Potable (0) oranlarını gösteren etkileşimli pasta grafiği (`px.pie(...)` çıktısı) kullanılmıştır. Bu görsel, veri setindeki sınıfların dengesizliğini tespit etmeye ve model seçimini bu duruma göre yapmaya olanak sağlamıştır.

🔹 Özellik Dağılım Karşılaştırmaları

İçilebilir ve içilemez suların her bir kimyasal özellik (pH, Sertlik, Sülfat vb.) için ayrı ayrı histogram karşılaştırmaları yapılmıştır.

---

🧠 Makine Öğrenimi Süreci ve Sonuçlar

Kullanılan Modeller:

1.  *DecisionTreeClassifier*
2.  *RandomForestClassifier*

Model performansları, RandomizedSearchCV ve RepeatedStratifiedKFold optimizasyonları sonrasında karşılaştırılmıştır:

| Model | Precision (Hassasiyet) | Stabilite |
| :--- | :--- | :--- |
| **Decision Tree** | 0.72 | Orta |
| **Random Forest** | **0.79** | Yüksek |

> Analiz Sonucu: Random Forest modeli, çapraz doğrulama teknikleri sayesinde daha iyi genelleme performansı ve daha yüksek bir hassasiyet (Precision) skoru göstermiştir. Bu, projenin nihai tahmin modeli olarak seçilmiştir.

---

🎯 Bu Projede Gösterilen Yetkinlikler

✅ Veri Temizleme ve Yönetimi: Eksik verinin tespiti ve stratejik olarak doldurulması.
✅ İleri Görselleştirme: Etkileşimli (Plotly) ve analitik (Seaborn) görselleştirmeleri etkin kullanma.
✅ Makine Öğrenimi Mühendisliği: Model geliştirme, hiperparametre optimizasyonu ve çapraz doğrulama uygulamaları.
✅ Değerlendirme Bilinci: Sınıflandırma problemlerinde doğru metrikleri (Precision, Confusion Matrix) kullanma.
✅ Profesyonel Proje Akışı: Google Colab üzerinde düzenli, yeniden üretilebilir (reproducible) kod yapısı oluşturma.

---

📬 İletişim

* 📧 **E-posta**: dogukansark44@gmail.com
* 🌐 **GitHub**: [github.com/onlyDogukan4](https://github.com/onlyDogukan4)
* 💼 **LinkedIn**: [linkedin.com/in/dogukansark] https://linkedin.com/in/dogukansark](https://www.linkedin.com/in/do%C4%9Fukan-%C5%9Fark-95658327a/
