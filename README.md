# 🌌 MAGIC Gamma Telescope: Makine Öğrenmesi ile Sinyal Sınıflandırma

Bu proje, Gazi Üniversitesi Bilgisayar Mühendisliği Veri Bilimi dersi kapsamında hazırlanmış kapsamlı bir dönem projesidir. Uzaydan gelen sinyallerin (Gama ışınları vs. Hadron gürültüleri) makine öğrenmesi ve derin öğrenme algoritmaları kullanılarak filtrelenmesini amaçlamaktadır.

## 🎯 Projenin Amacı
MAGIC (Major Atmospheric Gamma Imaging Cherenkov) teleskoplarından elde edilen veriler kullanılarak, gerçek gama sinyallerini yüksek duyarlılıkla (Recall) yakalamak ve teleskop zamanı israfını önlemek için otomatik bir sınıflandırma sistemi (AI Filtresi) geliştirilmiştir.

## 🚀 Projenin Özgün Değerleri
1. **Veri Sızıntısı (Data Leakage) Önleme:** SMOTE (Sentetik Veri Üretimi) işlemi, Imblearn Pipeline mimarisi içine gömülerek Cross-Validation sızıntıları sıfıra indirilmiştir.
2. **Kapsamlı Model Kıyaslaması:** 6 farklı klasik makine öğrenmesi modeli (Lojistik Regresyon, KNN, Karar Ağaçları, Random Forest, Naive Bayes) ve bir Yapay Sinir Ağı (YSA) mimarisi test edilmiştir.
3. **Açıklanabilir Yapay Zeka (XAI):** SHAP analizi ile Random Forest modelinin kararları hem global hem de lokal düzeyde şeffaflaştırılmıştır.
4. **Hiperparametre Optimizasyonu:** RandomizedSearchCV ile ezberleme (overfitting) riski önlenerek genelleme gücü en yüksek ağırlıklar bulunmuştur.

## 📁 Klasör Yapısı
* `/1_Code`: Model eğitimi, veri ön işleme, SMOTE ve SHAP analizlerini içeren Python kaynak kodları (Colab Notebook).
* `/2_Report`: Projenin tüm metodolojik adımlarını, literatür taramasını ve matematiksel gerekçelerini içeren akademik rapor.
* `/3_Presentation`: Görsel sunum dosyası.


## 🏆 Sonuçlar
Lider model olan **Optimize Edilmiş Rastgele Orman (Random Forest)**, SMOTE entegrasyonu ile dengesiz veri problemini aşmış ve özellikle azınlık sınıfı olan Hadron sinyallerini yakalamada (Recall) büyük bir başarı göstermiştir. Gözetimsiz öğrenme (K-Means) analizleri sonucunda ARI skorunun 0.0076 çıkması, problemin doğrusal olmayan doğasını ve gözetimli modellerin zorunluluğunu matematiksel olarak kanıtlamıştır.

---
*Geliştirici:* [SUDE AKSU] [ ELİF KINALI] - Gazi Üniversitesi Bilgisayar Mühendisliği Öğrencisi