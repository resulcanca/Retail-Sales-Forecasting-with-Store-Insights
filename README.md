# Retail Sales Forecasting with Store Insights

## 🎯 Proje Amacı
Bu projede, Rossmann mağazalarının günlük satış verileri kullanılarak gelecekteki satışlar tahmin edilmiştir. Mağaza bilgileri, promosyon detayları ve tarihsel veriler birleştirilerek anlamlı özellikler oluşturulmuş, ardından makine öğrenmesi modelleri ile satış tahminleri gerçekleştirilmiştir.

## 📊 Kullanılan Veri Setleri
- **train.csv**: Geçmiş satış verileri (mağaza, tarih, promosyon, tatil durumu vb.)
- **store.csv**: Mağazalara ait sabit bilgiler (mağaza tipi, konumu, rekabet mesafesi vb.)
- **test.csv**: Tahmin yapılacak tarih aralıkları
- **sample_submission.csv**: Kaggle için beklenen tahmin formatı

## ⚙️ Uygulanan Adımlar
1. Verilerin yüklenmesi ve ilk incelemesi  
2. Mağaza bilgileri ile satış verilerinin birleştirilmesi (merge)  
3. Tarih sütunundan yeni özellikler oluşturulması (Yıl, Ay, Haftanın haftası vb.)  
4. Kategorik değişkenlerin sayısal hale getirilmesi (encoding)  
5. Eksik verilerin medyan ile doldurulması  
6. **Random Forest Regressor** modeli ile eğitim  
7. Satış tahminlerinin yapılması ve Kaggle formatında submission dosyasının oluşturulması  

## 📈 Kullanılan Model
- **Model:** RandomForestRegressor  
- **Neden?** Karmaşık veri yapılarında hızlı, güçlü ve yorumlanabilir sonuçlar sunması  
- **Alternatif Modeller:** XGBoost, LightGBM (ileride test edilmek üzere)  

## 🔚 Sonuç
Model, mağaza ve tarihsel bilgiler kullanılarak satış tahminleri yapabilir hale getirilmiştir. Üretilen submission dosyası Kaggle yarışması için uygun formatta oluşturulmuştur. Model performansı ilerleyen süreçte farklı algoritmalar ve optimizasyon yöntemleri ile artırılabilir.
