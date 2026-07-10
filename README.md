# 🏡 Ames Housing Price Prediction (Advanced Regression Techniques)

Bu proje; Iowa'nın Ames şehrindeki konutların yapısal, konumsal ve dönemsel özelliklerini analiz ederek ev fiyatlarını tahmin etmeyi amaçlayan gelişmiş bir **Makine Öğrenmesi (Machine Learning)** projesidir. Veri bilimi yaşam döngüsüne (Data Science Lifecycle) uygun olarak uçtan uca bir boru hattı (Pipeline) mimarisi uygulanmıştır.

---

## 🛠️ Uygulanan Veri Bilimi Aşamaları

### 1. Keşifsel Veri Analizi (EDA) & Eksik Veri Yönetimi
- Veri setindeki yapısal özellikler incelenmiş, eksik verilerin (Missing Values) genel veri setine oranı matematiksel olarak hesaplanmıştır.
- Eksik veriler, veri kaybını önlemek adına nümerik alanlarda medyan (median) değerleri ile doldurulmuş; kategorik alanlar ise yapısal bütünlüğü koruyacak şekilde izole edilmiştir.

### 2. Özellik Mühendisliği (Feature Engineering)
- Model karmaşıklığını optimize etmek amacıyla Train ve Test veri kümeleri dikey eksende (`pd.concat`) birleştirilerek tek tip veri ön işleme hattına tabi tutulmuştur.
- Kategorik değişkenler, algoritmaların yüksek performansla çalışabilmesi için `LabelEncoder` teknikleriyle nümerik uzaya haritalandırılmıştır.

### 3. Topluluk Öğrenmesi (Ensemble Learning) ve Modelleme
Regresyon başarısını en üst seviyeye çıkarmak ve aşırı öğrenmeyi (Overfitting) engellemek amacıyla sektör standardı güçlü Gradient Boosting algoritmaları entegre edilmiştir:
- 🚀 **XGBoost Regressor (`XGBRegressor`)**
- ⚡ **LightGBM Regressor (`LGBMRegressor`)**

---

## 🏗️ Proje Yapısı
```text
Ames-Housing-Price-Prediction/
│
├── ameshouse.ipynb     # EDA, Veri Ön İşleme ve Model Eğitim Jupyter Notebook'u
└── README.md           # Proje dökümantasyonu
```

🚀 Kullanılan Teknolojiler ve Kütüphaneler
  Python 3.x
  Veri Analizi & Manipülasyon: Pandas, NumPy
  Makine Öğrenmesi Framework'leri: Scikit-Learn, XGBoost, LightGBM
  Geliştirme Ortamı: Jupyter Notebook

🔧 Kurulum ve Çalıştırma
1. Gerekli Kütüphanelerin Kurulması
Projeyi yerel bilgisayarınızda çalıştırmak için öncelikle terminal üzerinden gerekli veri bilimi bağımlılıklarını yükleyin:
```bash
pip install pandas numpy scikit-learn xgboost lightgbm jupyter
```

2. Jupyter Notebook'un Başlatılması
Depoyu bilgisayarınıza klonlayın:
```bash
git clone [https://github.com/FarukSelman/Ames-Housing-Price-Prediction.git](https://github.com/FarukSelman/Ames-Housing-Price-Prediction.git)
```
Proje klasörünün içine girin ve Jupyter laboratuvarını başlatın:
```bash
cd Ames-Housing-Price-Prediction
jupyter notebook
```
Tarayıcıda açılan arayüz üzerinden ameshouse.ipynb dosyasını seçerek tüm hücreleri sırasıyla (Run All) çalıştırabilirsiniz.

💡 Bu proje; yüksek boyutlu veri kümelerinde eksik veri stratejileri geliştirme, kategorik dönüşüm optimizasyonları ve topluluk (ensemble) tabanlı gradyan artırma algoritmaları ile tahminsel modelleme süreçlerini deneyimlemek amacıyla geliştirilmiştir.
