🏪 Retail Sales Forecasting with Store Insights¶
🎯 Proje Amacı
Bu projede, Rossmann mağazalarının satış verileri kullanılarak günlük satış tahminleri yapılmıştır. Mağaza bilgileri, promosyon detayları ve tarihsel veriler birleştirilerek anlamlı özellikler oluşturulmuş; makine öğrenmesi modelleriyle gelecekteki satışlar tahmin edilmiştir.

📊 Kullanılan Veri Setleri
train.csv: Geçmiş satış verileri (mağaza, tarih, promosyon, tatil vs.)
store.csv: Her mağaza için sabit bilgiler (tipi, konumu, rekabet mesafesi vs.)
test.csv: Tahmin yapılacak tarihler
sample_submission.csv: Beklenen tahmin formatı
⚙️ Uygulanan Adımlar
Veri Yükleme & İnceleme
Mağaza bilgileriyle birleştirme (merge)
Tarih sütunundan yeni özellikler üretme (Year, Month, WeekOfYear vs.)
Kategorik değişkenleri encoding ile sayısallaştırma
Eksik verilerin medyanla doldurulması
Random Forest Regressor ile model eğitimi
Satış tahminlerinin yapılması ve submission dosyası oluşturulması
📈 Kullanılan Model
Model: RandomForestRegressor
Neden?: Karmaşık veri setlerinde hızlı, güçlü ve yorumlanabilir sonuçlar sunması
Alternatifler: XGBoost, LightGBM (ileride test edilebilir)
🔚 Sonuç
Model, mağaza ve tarihsel bilgilerle tahmin yapabilecek duruma getirildi. Submission dosyası Kaggle yarışması için uygun formatta üretildi. Performans daha ileri modellerle artırılabilir.
