# Yapay Zeka Temelleri - Meme Kanseri Teşhisi ve Sınıflandırması

Bu proje, Makine Öğrenmesi algoritmaları kullanılarak hücre çekirdeği özelliklerine bakılıp bir tümörün iyi huylu (benign) veya kötü huylu (malignant) olup olmadığını tahmin etmeyi amaçlamaktadır. Projede veri analizi, görselleştirme, model eğitimi ve performans değerlendirmesi adımları uçtan uca uygulanmıştır.

## Projenin Amacı
Sağlık alanında makine öğrenmesi yaklaşımlarının teşhis süreçlerine nasıl entegre edilebileceğini göstermektir. 30 farklı sayısal hücre özelliği (yarıçap, doku, pürüzsüzlük vb.) analiz edilerek yüksek doğruluk oranına sahip bir sınıflandırma modeli geliştirmek hedeflenmiştir. Sınıflandırma problemi olarak ele alınmıştır.

## Kullanılan Veri Seti ve Kaynağı
Projede **Kaggle** platformunda da yaygın olarak kullanılan ve Scikit-learn kütüphanesine entegre edilmiş olan "Breast Cancer Wisconsin (Diagnostic)" veri seti kullanılmıştır. Veri setinde 569 adet hastaya ait 30'ar özellik bulunmaktadır. [cite_start]Eksik veri analizi yapılmış olup[cite: 27], verilerin temiz ve analize uygun olduğu saptanmıştır.
* **Kaynak Linki:** [Kaggle - Breast Cancer Wisconsin Data](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data)

## Kullanılan Teknolojiler ve Algoritma
* **Programlama Dili:** Python
* [cite_start]**Veri Analizi ve Görselleştirme:** Pandas, NumPy, Matplotlib, Seaborn [cite: 30]
* [cite_start]**Makine Öğrenmesi Algoritması:** Rastgele Orman (Random Forest Classifier). Karar ağaçlarının topluluk halinde çalışmasını sağlayarak yüksek performans sunduğu için tercih edilmiştir.

## Model Değerlendirmesi ve Elde Edilen Sonuçlar
Model, veri setinin %20'si (test seti) üzerinde değerlendirilmiş ve aşağıdaki yüksek performans metriklerine ulaşılmıştır:

* [cite_start]**Accuracy (Doğruluk):** 0.9649 [cite: 48]
* [cite_start]**Precision (Kesinlik):** 0.9589 [cite: 49]
* [cite_start]**Recall (Duyarlılık):** 0.9859 
* [cite_start]**F1 Skoru:** 0.9722 [cite: 51]

Elde edilen %96.49'luk doğruluk oranı, modelin tıbbi bir veri seti üzerinde oldukça başarılı çalıştığını, tümörleri teşhis ederken yanıltıcı sonuç (False Positive/Negative) üretme ihtimalinin çok düşük olduğunu kanıtlamaktadır.
