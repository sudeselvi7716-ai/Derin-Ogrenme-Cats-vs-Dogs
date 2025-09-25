# Derin-Ogrenme-Cats-vs-Dogs
CNN kullanarak kedi ve köpek görüntülerini sınıflandırma projesi.
# 🚀 CNN Tabanlı Görüntü Sınıflandırma Projesi: Kedi ve Köpek Sınıflandırması

## 🎯 Projenin Amacı
Bu proje, **Evrişimli Sinir Ağları (CNN)** mimarisi kullanarak bir derin öğrenme modeli geliştirmeyi ve bu modelin kedi ile köpek görüntülerini yüksek doğrulukla sınıflandırmasını amaçlamaktadır. Proje, görüntü analizi, veri çoğaltma (Data Augmentation) ve model yorumlama (Grad-CAM) konularında pratik deneyim sağlamıştır.

## 📁 Veri Seti Hakkında Bilgi
* **Veri Seti Adı:** Microsoft Cats vs Dogs Dataset
* **İçerik:** [Açıklama: Veri seti, iki sınıfa (Kedi ve Köpek) ait binlerce görüntü içerir.]
* **Ön İşleme:** Görüntüler (128x128x3) boyutuna yeniden ölçeklendirilmiş ve 0-1 aralığına normalize edilmiştir. Overfitting'i önlemek ve modelin genelleme yeteneğini artırmak için **Data Augmentation** yöntemleri (Rotasyon, Yatay Çevirme, Zoom) kullanılmıştır.

## 🛠️ Kullanılan Yöntemler ve Mimariler
* **Model Tipi:** Ardışık (Sequential) CNN Mimarisi
* **Bileşenler:** Convolutional Layers, MaxPooling Layers, GlobalAveragePooling, Dropout (Overfitting'i azaltmak için 0.4), Dense Layers.
* **Aktivasyon Fonksiyonları:**  ReLU ve çıkış katmanında Sigmoid.
* **Optimizasyon:**  Adam Optimizer ve  0.001.
* **Hiperparametre Optimizasyonu:** 15 deneme yapılmış ve Katman sayısı optimize edilmiştir.

## ✅ Elde Edilen Sonuçlar
* **Final Model Doğruluğu (Accuracy):** ** %84 **
* **Model Durumu:** Model, Eğitim/Doğrulama Kaybı grafikleri incelendiğinde, **minimal/az** overfit göstermiş ve başarılı bir şekilde genelleme yapmıştır.
* **Model Yorumlama (Grad-CAM):** Grad-CAM görselleştirmesi, modelin sınıflandırma kararlarını verirken, kedi ve köpeklerin yüz ve vücut hatları gibi **anlamsal olarak doğru bölgelere** odaklandığını göstermiştir.

## 🔗 Kaggle Notebook Linki
Projenin tüm kodları, görselleri ve detaylı çıktıları aşağıdaki Kaggle notebook'unda bulunmaktadır:

**https://www.kaggle.com/code/sudeslvii/fork-of-notebook6007f7cc6f**
