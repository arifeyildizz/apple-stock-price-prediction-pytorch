# 📈 Apple Hisse Senedi Fiyat Tahmini (LSTM & GRU) | PyTorch

## 📌 Proje Hakkında

Bu proje, Apple Inc. (AAPL) hisse senedi kapanış fiyatlarını geçmiş verilerden yararlanarak tahmin etmek amacıyla geliştirilmiştir. Projede derin öğrenme tabanlı **LSTM (Long Short-Term Memory)** ve **GRU (Gated Recurrent Unit)** modelleri kullanılmıştır.

Veriler Yahoo Finance üzerinden alınmış, ön işleme adımları uygulanmış ve PyTorch kütüphanesi kullanılarak modeller eğitilmiştir. Elde edilen tahmin sonuçları gerçek veriler ile karşılaştırılmış ve modellerin performansı **MSE (Mean Squared Error)** ve **RMSE (Root Mean Squared Error)** metrikleri ile değerlendirilmiştir.

---

# 🎯 Projenin Amacı

Bu projenin amacı;

- Zaman serisi verilerinin analiz edilmesi,
- Hisse senedi fiyat tahmini için derin öğrenme modellerinin uygulanması,
- LSTM ve GRU modellerinin performanslarının karşılaştırılması,
- PyTorch ile gerçek dünya problemlerine yönelik makine öğrenmesi uygulaması geliştirmektir.

---

# 🛠 Kullanılan Teknolojiler

- Python
- PyTorch
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- yfinance
- Jupyter Notebook

---

# 📊 Kullanılan Veri Seti

Veri seti Yahoo Finance platformundan **Apple Inc. (AAPL)** hisse senedi verileri kullanılarak elde edilmiştir.

Veri içerisinde;

- Açılış Fiyatı (Open)
- Kapanış Fiyatı (Close)
- En Yüksek Fiyat (High)
- En Düşük Fiyat (Low)
- İşlem Hacmi (Volume)

bilgileri bulunmaktadır.

Bu projede model eğitimi için **Kapanış Fiyatı (Close Price)** kullanılmıştır.

---

# ⚙ Veri Ön İşleme

Model eğitimi öncesinde aşağıdaki işlemler uygulanmıştır.

- Veri setinin indirilmesi
- Eksik verilerin kontrol edilmesi
- Kapanış fiyatlarının seçilmesi
- Min-Max Normalizasyonu
- Eğitim ve Test verisinin ayrılması
- Sliding Window yöntemi ile zaman serisi oluşturulması

---

# 🧠 Kullanılan Derin Öğrenme Modelleri

## ✅ LSTM (Long Short-Term Memory)

LSTM modeli zaman serilerindeki uzun dönemli bağımlılıkları öğrenmek amacıyla kullanılmıştır.

Model;

- 2 Katmanlı LSTM
- Adam Optimizer
- MSE Loss
- 50 Epoch

ile eğitilmiştir.

---

## ✅ GRU (Gated Recurrent Unit)

GRU modeli daha az parametre ile hızlı öğrenme sağlayan bir RNN mimarisidir.

Aynı veri üzerinde eğitilerek LSTM modeli ile performans karşılaştırması yapılmıştır.

---

# 📈 Performans Değerlendirme

Modeller aşağıdaki metrikler kullanılarak değerlendirilmiştir.

- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)

Ayrıca;

- Eğitim Loss Grafikleri
- Gerçek ve Tahmin Edilen Fiyat Grafikleri

oluşturulmuştur.

---

# 📁 Proje Yapısı

```
StockPricePrediction/
│
├── notebooks/
│   └── StockPrediction.ipynb
|   └── AAPL.csv
│
├── models/
│   ├── lstm_model.pth
│   └── gru_model.pth
│
├── results/
│ 
│   ├── model_results.csv
│   └── model_report.txt
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# 🚀 Kurulum

Projeyi bilgisayarınıza klonlayın.

```bash
git clone https://github.com/KULLANICI_ADIN/apple-stock-price-prediction-pytorch.git
```

Proje klasörüne girin.

```bash
cd apple-stock-price-prediction-pytorch
```

Gerekli kütüphaneleri yükleyin.

```bash
pip install -r requirements.txt
```

Notebook'u çalıştırın.

```bash
jupyter notebook
```

---

# 📊 Çıktılar

Proje sonunda;

- Eğitilmiş LSTM modeli
- Eğitilmiş GRU modeli
- Tahmin Grafikleri
- Eğitim Loss Grafikleri
- MSE ve RMSE Sonuçları

elde edilmektedir.

---

# 💡 Gelecekte Yapılabilecek Geliştirmeler

- Farklı hisse senetleri için destek eklenmesi
- Transformer tabanlı modellerin uygulanması
- Attention Mechanism kullanılması
- Hyperparameter Optimization
- Streamlit ile web arayüzü geliştirilmesi
- Gerçek zamanlı veri ile tahmin yapılması

---

# 👩‍💻 Geliştirici

**Arife Yıldız**

Büyük Veri Analistliği Öğrencisi

İlgi Alanları

- Veri Analizi
- Veri Bilimi
- Büyük Veri
- Yapay Zeka
- Derin Öğrenme
- Makine Öğrenmesi

---

# ⭐ Not

Bu proje eğitim amacıyla geliştirilmiş olup finansal yatırım tavsiyesi niteliği taşımamaktadır.
