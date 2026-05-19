# Telco Customer Churn Sınıflandırma Projesi

Bu proje, telekomünikasyon müşterilerinin churn (ayrılma) olasılığını tahmin etmek için uçtan uca bir veri madenciliği çalışması sunar. Çalışma; veri temizleme, keşifsel veri analizi (EDA), özellik mühendisliği, farklı model denemeleri ve SMOTE ile sınıf dengesizliği yönetimini kapsar.

## Proje Özeti

- Problem: Müşterinin hizmetten ayrılıp ayrılmayacağını tahmin etmek
- Veri seti: IBM Telco Customer Churn veri seti
- Hedef değişken: `Churn`
- Yaklaşım: EDA + özellik mühendisliği + model karşılaştırma + dengeleme (SMOTE)

## Dosya Yapısı

- `Proje.ipynb`: Tüm analiz, görselleştirme ve modelleme adımları
- `WA_Fn-UseC_-Telco-Customer-Churn.csv`: Ham veri seti

## Kullanım Senaryosu

Bu notebook, şu sorulara yanıt vermeyi hedefler:

- Hangi müşteri segmentlerinde churn riski daha yüksek?
- Hangi değişkenler churn ile daha güçlü ilişki gösteriyor?
- Hangi model/ölçekleme kombinasyonu daha iyi performans veriyor?
- Sınıf dengesizliği giderildiğinde model davranışı nasıl değişiyor?

## Yöntem ve İş Akışı

1. Veri yükleme ve ilk inceleme
2. Veri temizleme ve dönüşümler
3. EDA (dağılımlar, churn bazlı karşılaştırmalar, grafikler)
4. Özellik mühendisliği (servis sayısı, müşteri değeri, churn risk skoru vb.)
5. Model karşılaştırma:
	- Logistic Regression
	- Random Forest
	- SVM
6. Sınıf dengesizliği için SMOTE
7. Final değerlendirme (accuracy, confusion matrix, classification report)

## Öne Çıkan Bulgular

- Notebook çıktılarında churn oranı yaklaşık `%26.5` seviyesindedir.
- Farklı ölçekleme seçenekleri altında model karşılaştırması yapılmıştır.
- SMOTE sonrası eğitim seti dengelenmiş ve final model değerlendirmesi yapılmıştır.

Not: Son metrikler notebook hücrelerinin yeniden çalıştırılmasına göre değişebilir.

## Kullanılan Teknolojiler

- Python 3.x
- Jupyter Notebook / VS Code Notebook
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- imbalanced-learn (SMOTE)

## Kurulum

1. Depoyu klonlayın:

```bash
git clone https://github.com/yildirimyusuf79/Veri-Madencili-i-Projesi.git
cd Veri-Madencili-i-Projesi
```

2. Bağımlılıkları kurun:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter
```

3. Notebook'u açın:

```bash
jupyter notebook Proje.ipynb
```

## Tekrar Üretilebilirlik

- Notebook hücrelerini üstten alta sırayla çalıştırınız.
- Rastgelelik içeren adımlarda `random_state=42` kullanılmıştır.
- Sonuçların birebir aynı olması için benzer kütüphane sürümleri önerilir.

## Geliştirme Fikirleri

- Hyperparameter tuning (GridSearchCV / RandomizedSearchCV)
- ROC-AUC, PR-AUC gibi ek metriklerle detaylı değerlendirme
- Model yorumlanabilirliği (SHAP, feature importance analizi)
- Pipeline yapısı ile daha modüler ve temiz deney akışı

## Lisans ve Kaynak

Bu çalışma eğitsel amaçlarla hazırlanmıştır. Veri seti, Telco Customer Churn açık veri kaynağına dayanmaktadır.

## İletişim

- GitHub: [github.com/yildirimyusuf79](https://github.com/yildirimyusuf79)
- LinkedIn: [www.linkedin.com/in/yusuf-yıldırım-190445295](https://www.linkedin.com/in/yusuf-yıldırım-190445295)
