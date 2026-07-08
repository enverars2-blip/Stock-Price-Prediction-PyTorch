# Stock Price Prediction with PyTorch (LSTM vs GRU)

Bu proje, PyTorch kütüphanesi kullanılarak Amazon (AMZN) şirketi hisse senedi fiyatlarının derin öğrenme modelleri (LSTM ve GRU) ile tahmin edilmesini ve performanslarının karşılaştırılmasını içerir.

This project implements and compares LSTM and GRU deep learning models using PyTorch to predict Amazon (AMZN) stock prices based on historical time-series data.

## 📊 Sonuçlar ve Karşılaştırma (Results & Comparison)

Modeller 50 epoch boyunca eğitilmiş ve daha önce hiç görülmemiş test verisi üzerinde test edilmiştir:
The models were trained for 50 epochs and evaluated on unseen test data:

| Model | Test MSE (Hata Değeri) | Performans (Performance) |
| :--- | :---: | :---: |
| **GRU** | **26.5950** | En İyi Sonuç (Best Performer) |
| **LSTM** | 80.0885 | Daha Yüksek Hata (Higher Error) |

### 🔑 Ana Çıkarımlar (Key Takeaways)
* GRU modeli, borsa verisindeki ani dalgalanmaları ve trendleri LSTM'e göre daha az hata ile öğrenmiştir.
* Zaman serisi tahminlerinde GRU'nun daha azampatılı mimarisi bu veri setinde çok daha kararlı sonuçlar üretmiştir.
* (The GRU model outperformed the LSTM model on this dataset, capturing the price trends with a significantly lower Mean Squared Error.)

## 🛠️ Kullanılan Teknolojiler (Tech Stack)
* Python 3
* PyTorch (Deep Learning Framework)
* Pandas & Numpy (Data Manipulation)
* Matplotlib (Data Visualization)
* Scikit-Learn (MinMax Scaling)
