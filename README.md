# Telco Customer Churn Siniflandirma Projesi

Bu proje, telekomunikasyon musterilerinin churn (ayrilma) olasiligini tahmin etmek icin uctan uca bir veri madenciligi calismasi sunar. Calisma; veri temizleme, kesifsel veri analizi (EDA), ozellik muhendisligi, farkli model denemeleri ve SMOTE ile sinif dengesizligi yonetimini kapsar.

## Proje Ozeti

- Problem: Musterinin hizmetten ayrilip ayrilmayacagini tahmin etmek
- Veri seti: IBM Telco Customer Churn veri seti
- Hedef degisken: `Churn`
- Yaklasim: EDA + ozellik muhendisligi + model karsilastirma + dengeleme (SMOTE)

## Dosya Yapisi

- `Proje.ipynb`: Tum analiz, gorsellestirme ve modelleme adimlari
- `WA_Fn-UseC_-Telco-Customer-Churn.csv`: Ham veri seti

## Kullanim Senaryosu

Bu notebook, su sorulara yanit vermeyi hedefler:

- Hangi musteri segmentlerinde churn riski daha yuksek?
- Hangi degiskenler churn ile daha guclu iliski gosteriyor?
- Hangi model/olcekleme kombinasyonu daha iyi performans veriyor?
- Sinif dengesizligi giderildiginde model davranisi nasil degisiyor?

## Yontem ve Is Akisi

1. Veri yukleme ve ilk inceleme
2. Veri temizleme ve donusumler
3. EDA (dagilimlar, churn bazli karsilastirmalar, grafikler)
4. Ozellik muhendisligi (servis sayisi, musteri degeri, churn risk skoru vb.)
5. Model karsilastirma:
	- Logistic Regression
	- Random Forest
	- SVM
6. Sinif dengesizligi icin SMOTE
7. Final degerlendirme (accuracy, confusion matrix, classification report)

## One Cikan Bulgular

- Notebook ciktilarinda churn orani yaklasik `%26.5` seviyesindedir.
- Farkli olcekleme secenekleri altinda model karsilastirmasi yapilmistir.
- SMOTE sonrasi egitim seti dengelenmis ve final model degerlendirmesi yapilmistir.

Not: Son metrikler notebook hucrelerinin yeniden calistirilmasina gore degisebilir.

## Kullanilan Teknolojiler

- Python 3.x
- Jupyter Notebook / VS Code Notebook
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- imbalanced-learn (SMOTE)

## Kurulum

1. Depoyu klonlayin:

```bash
git clone https://github.com/yildirimyusuf79/Veri-Madencili-i-Projesi.git
cd Veri-Madencili-i-Projesi
```

2. Bagimliliklari kurun:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn jupyter
```

3. Notebook'u acin:

```bash
jupyter notebook Proje.ipynb
```

## Tekrar Uretilebilirlik

- Notebook hucrelerini ustten alta sirayla calistiriniz.
- Rastgelelik iceren adimlarda `random_state=42` kullanilmistir.
- Sonuclarin birebir ayni olmasi icin benzer kutuphane surumleri onerilir.

## Gelistirme Fikirleri

- Hyperparameter tuning (GridSearchCV / RandomizedSearchCV)
- ROC-AUC, PR-AUC gibi ek metriklerle detayli degerlendirme
- Model yorumlanabilirligi (SHAP, feature importance analizi)
- Pipeline yapisi ile daha moduler ve temiz deney akisi

## Lisans ve Kaynak

Bu calisma egitsel amaclarla hazirlanmistir. Veri seti, Telco Customer Churn acik veri kaynagina dayanmaktadir.

## Iletisim

- GitHub: [github.com/yildirimyusuf79](https://github.com/yildirimyusuf79)
- LinkedIn: [www.linkedin.com/in/yusuf-yıldırım-190445295](https://www.linkedin.com/in/yusuf-yıldırım-190445295)
