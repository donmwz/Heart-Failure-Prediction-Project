Heart Failure Prediction Projesi

Bu kod, kalp hastalığı (HeartDisease) tahmini yapmak için üç farklı makine öğrenmesi modeli uygular:
- Logistic Regression (Lojistik Regresyon)
- Random Forest (Rastgele Orman)
- XGBoost (Extreme Gradient Boosting)

Veri seti (heart.csv) şu özellikleri içerir:
- Age: Yaş
- Sex: Cinsiyet (M/F)
- ChestPainType: Göğüs ağrısı tipi (ATA, NAP, ASY, TA)
- RestingBP: Dinlenme kan basıncı
- Cholesterol: Kolesterol seviyesi
- FastingBS: Açlık kan şekeri (0=normal, 1=yüksek)
- RestingECG: Dinlenme elektrokardiyografi sonucu
- MaxHR: Maksimum kalp hızı
- ExerciseAngina: Egzersiz sırasında görülen anjina (N=Hayır, Y=Evet)
- Oldpeak: Egzersiz sonrası ST depresyonu
- ST_Slope: ST segmentinin eğimi
- HeartDisease: Kalp hastalığı varlığı (0=Yok, 1=Var) — hedef değişken

Kodda kategorik veriler sayısal hale dönüştürülmek için LabelEncoder kullanılmıştır.
Veri eğitim ve test olarak %80-%20 oranında bölünmüştür.
Her model ayrı ayrı eğitilir ve test setinde değerlendirilmiştir.
Değerlendirme metrikleri olarak Accuracy, Confusion Matrix ve Classification Report kullanılmıştır.

Amaç, hangi modelin kalp hastalığını tahmin etmede daha başarılı olduğunu karşılaştırmaktır.
"""
