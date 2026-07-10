# 🏡 Ames Housing Price Prediction (Advanced Regression Techniques)

Bu proje, Iowa'nın Ames şehrindeki konutların yapısal, konumsal ve zamansal özelliklerini analiz ederek ev satış fiyatlarını tahmin etmeyi amaçlayan gelişmiş bir **Makine Öğrenmesi (Machine Learning) Regresyon** çalışmasıdır. Projede veri ön işleme, eksik veri yönetimi, özellik mühendisliği ve modern gradient boosting algoritmaları kullanılarak uçtan uca bir makine öğrenmesi pipeline'ı oluşturulmuştur.

---

# 🛠️ Uygulanan Veri Bilimi Aşamaları

## 1. Keşifsel Veri Analizi (EDA) & Eksik Veri Yönetimi

Model eğitiminden önce veri seti ayrıntılı olarak analiz edilmiştir.

Uygulanan işlemler:

- Veri tiplerinin incelenmesi
- Eksik değer oranlarının hesaplanması
- Sayısal değişkenlerde eksik değerlerin **median** ile doldurulması
- Kategorik değişkenlerin uygun yöntemlerle işlenmesi
- Veri tutarlılığının kontrol edilmesi

Bu işlemler veri kaybını önleyerek model performansını artırmayı amaçlamaktadır.

---

## 2. Özellik Mühendisliği (Feature Engineering)

Modelleme sürecinde eğitim ve test veri setlerine aynı dönüşümlerin uygulanabilmesi amacıyla ortak bir ön işleme hattı oluşturulmuştur.

Uygulanan işlemler:

- Train ve Test veri setlerinin birleştirilmesi (`pd.concat`)
- Kategorik değişkenlerin **Label Encoding** yöntemiyle sayısal değerlere dönüştürülmesi
- Model eğitimine uygun veri yapısının oluşturulması

---

## 3. Modelleme (Regression Models)

Ev fiyatlarını tahmin etmek amacıyla iki güçlü gradient boosting algoritması kullanılmıştır.

Kullanılan modeller:

- 🚀 XGBoost Regressor (XGBRegressor)
- ⚡ LightGBM Regressor (LGBMRegressor)

Her iki model de aynı veri üzerinde eğitilmiş ve regresyon performansları karşılaştırılmıştır.

---

# 📊 Kullanılan Performans Metrikleri

Modeller aşağıdaki regresyon metrikleri ile değerlendirilmiştir.

- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² Score (Coefficient of Determination)

Bu metrikler modelin tahmin doğruluğunu ve hata seviyesini değerlendirmek amacıyla kullanılmıştır.

---

# 🏗️ Proje Yapısı

```text
Ames-Housing-Price-Prediction/
│
├── ameshouse.ipynb     # Veri ön işleme, feature engineering ve model eğitimi
└── README.md           # Proje dokümantasyonu
```

---

# 🚀 Kullanılan Teknolojiler

## Programlama Dili

- Python 3.x

## Veri Analizi

- Pandas
- NumPy

## Makine Öğrenmesi

- Scikit-Learn
- XGBoost
- LightGBM

## Geliştirme Ortamı

- Jupyter Notebook

---

# 🔧 Kurulum

## 1. Repoyu Klonlayın

```bash
git clone https://github.com/FarukSelman/Ames-Housing-Price-Prediction.git
```

## 2. Proje Klasörüne Girin

```bash
cd Ames-Housing-Price-Prediction
```

## 3. Gerekli Kütüphaneleri Kurun

```bash
pip install pandas numpy scikit-learn xgboost lightgbm jupyter
```

## 4. Jupyter Notebook'u Başlatın

```bash
jupyter notebook
```

Ardından açılan arayüzden **ameshouse.ipynb** dosyasını açarak tüm hücreleri sırasıyla (**Run All**) çalıştırabilirsiniz.

---

# 📈 Proje Akışı

1. Veri setinin yüklenmesi
2. Keşifsel veri analizi (EDA)
3. Eksik değerlerin analiz edilmesi
4. Eksik verilerin doldurulması
5. Train ve Test veri setlerinin birleştirilmesi
6. Label Encoding uygulanması
7. Eğitim ve test veri setlerinin oluşturulması
8. XGBoost ve LightGBM modellerinin eğitilmesi
9. Ev fiyatı tahminlerinin oluşturulması
10. RMSE, MAE ve R² metrikleri ile model performansının değerlendirilmesi

---

# 💡 Projenin Amacı

Bu çalışma;

- Konut fiyatlarının makine öğrenmesi ile tahmin edilmesi,
- Eksik veri yönetimi stratejilerinin uygulanması,
- Özellik mühendisliği tekniklerinin kullanılması,
- Gradient boosting tabanlı regresyon modellerinin değerlendirilmesi,
- Gerçek dünya veri setleri üzerinde tahmin performansının artırılması

amacıyla geliştirilmiştir.

---

# 👨‍💻 Geliştirici

**Faruk Selman**

GitHub: https://github.com/FarukSelman
