# Face-Spoofing-Detection-DeepLearning
Deep learning project for face spoofing detection (binary classification: real vs fake). Colab-ready.


# 🧠 Yüz Sahteciliği Tespiti – Derin Öğrenme

Bu proje, **gerçek vs sahte yüz** ayrımı için derin öğrenme tabanlı bir ikili sınıflandırma modelidir.  
Birden fazla CNN mimarisi ve varyasyonu denenmiş; eğitim ve doğrulama doğrulukları karşılaştırılmıştır.

---

## 🎯 Amaç
- “Gerçek” ve “Sahte” sınıflarını ayıran bir model tasarlamak  
- Farklı mimari ve hiperparametrelerin doğruluğa etkisini gözlemlemek  
- Transfer öğrenme (VGG16, MobileNetV2) ile model performansını artırmak  

---

## ⚙️ Kullanılan Teknolojiler
- **Python 3.x**
- **TensorFlow / Keras**
- **NumPy, Pandas**
- **OpenCV**
- **Matplotlib**
- **scikit-learn**

---

## 📦 Veri Seti Yapısı
Veri seti Google Drive üzerinde iki klasör hâlinde tutulmuştur:
/real
/fake


Her klasör, etiketine karşılık gelen görüntüleri içerir.  
📌 **Veri seti GitHub’a yüklenmemiştir.**  
Kendi verini eklemek istersen aynı klasör yapısını koruyabilirsin.

---

## ☁️ Colab Uyumluluğu
Kod **Google Colab** üzerinde çalışacak şekilde yazılmıştır.  
Drive bağlantısı (`drive.mount`) ve Colab dosya yolları (`/content/drive/...`) hazırdır.

Eğer kodu bilgisayarında çalıştırmak istersen:
1. `real_path` ve `fake_path` değişkenlerini kendi veri yoluna göre düzenle (örneğin `data/real`, `data/fake`)  
2. Gerekli kütüphaneleri yükle:  
   ```bash
   pip install -r requirements.txt
    ```
3.Kodu çalıştır:  
   ```bash
     python face_spoofing_detection.py
   ```

### 🧪 Denenen Modeller

Basit CNN (ELU / Adadelta)

Aktivasyon değişimi (ReLU / Adam)

Dropout eklenmiş CNN

L2 regularizasyonlu CNN

Data augmentation (ImageDataGenerator)

Küçük hiperparametre değişiklikleri

Transfer Learning – VGG16

Transfer Learning – MobileNetV2


### 📈 Accuracy Gelişimi   

%59 → %85 → %64 → %60 → %51 → %62 → %81 → %96 → %98

### ▶️ Çalıştırma (Colab)

Drive’ı bağla (mount işlemi)

Kod dosyasını yükle

Hücreleri sırayla çalıştır

Eğitim / doğrulama sonuçlarını incele





# Face-Spoofing-Detection-DeepLearning
Deep learning project for **face spoofing detection** (binary classification: real vs fake). Colab-ready.

---

# 🧠 Face Spoofing Detection – Deep Learning

This project is a **deep learning-based binary classification model** for detecting **real vs fake faces**.  
Multiple CNN architectures and variations were tested, and training/validation accuracies were compared.

---

## 🎯 Objectives
- Design a model that distinguishes between “real” and “fake” faces  
- Observe the impact of different architectures and hyperparameters on accuracy  
- Improve performance through transfer learning (VGG16, MobileNetV2)

---

## ⚙️ Technologies Used
- **Python 3.x**
- **TensorFlow / Keras**
- **NumPy, Pandas**
- **OpenCV**
- **Matplotlib**
- **scikit-learn**

---

## 📦 Dataset Structure
The dataset is stored in Google Drive in two folders:
/real
/fake


Each folder contains images corresponding to its label.  
📌 **The dataset is not uploaded to GitHub.**  
You can add your own dataset while keeping the same folder structure.

---

## ☁️ Colab Compatibility
The code is written to work seamlessly in **Google Colab**.  
Drive mounting (`drive.mount`) and Colab file paths (`/content/drive/...`) are already included.

If you want to run it locally:
1. Update the `real_path` and `fake_path` variables according to your local directories (e.g., `data/real`, `data/fake`)  
2. Install the required dependencies:  
   ```bash
   pip install -r requirements.txt
3.Run the script:
```bash
   python face_spoofing_detection.py
```
### 🧪 Tested Models

Simple CNN (ELU / Adadelta)

Activation modification (ReLU / Adam)

CNN with Dropout

CNN with L2 Regularization

Data Augmentation (ImageDataGenerator)

Minor Hyperparameter Tweaks

Transfer Learning – VGG16

Transfer Learning – MobileNetV2

### 📈 Accuracy Progression

59% → 85% → 64% → 60% → 51% → 62% → 81% → 96% → 98%

### ▶️ Running on Colab

Mount your Google Drive

Upload the script

Run the cells sequentially

Review training and validation results
