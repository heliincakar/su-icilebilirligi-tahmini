# Su İçilebilirliği Tahmini

Bu projede suya ait fizikokimyasal ölçümler kullanılarak örneklerin içilebilirlik durumu tahmin edilmektedir. Çalışmada Logistic Regression, KNN, Random Forest ve XGBoost modelleri karşılaştırılmıştır.

## Dosyalar

- `su_kalitesi.ipynb`: Veri hazırlama, görselleştirme ve model karşılaştırma adımları.
- `su_icilebilirligi_raporu.pdf`: Notebook sonuçlarına göre güncellenen proje raporu.

## Kullanım

Önce gerekli paketleri kurun:

```bash
pip install -r requirements.txt
```

Ardından veri setini aşağıdaki kaynaktan indirip `water_potability.csv` adıyla proje klasörüne ekleyin. Sonra `su_kalitesi.ipynb` dosyasını Jupyter Notebook veya VS Code ile açıp hücreleri sırayla çalıştırın.

## Bulgular

Doğrulama verisinde en yüksek doğruluk Random Forest ile 0,664 olarak elde edilmiştir. İçilebilir sınıfın F1 skoru XGBoost modelinde 0,465 ile daha yüksektir. Bu sonuçlar, modellerin ön değerlendirme amacıyla kullanılabileceğini gösterse de nihai içilebilirlik kararı için laboratuvar analizinin gerekli olduğunu göstermektedir.

## Veri kaynağı

Water Potability veri seti: https://www.kaggle.com/datasets/uom190346a/water-quality-and-potability
