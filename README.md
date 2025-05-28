# Giriş

Amazon Ürünlerinin Tüketici Yorumları verisi üzerinde çalışmamı gerçekleştirdim.İlk olarak veriyi inceledim ardından benim için gerekli olan sütunlar üzerinde 
grafik dağılımlarını incelemeleye başladım.Sayısal değerler arasındaki korelasyonu inceledim veriler üzerinde incelemeleri gerçekleştirdim.
İkinci aşama olarak veriler üzerinde eksik verileri temizleme işlemi gerçekleştirdim ve aykırı değerleri inceledim.Makine öğrenmesi aşaması için etiket değeri belirleme ve kategorik verilere one-hot encoding işlemi uyguladım ardından standardizasyon aşamasını gerçekleştirerek makine öğrenmesine hazır hale getirdim.
Verileri train ve test olarak ayırdım verim için en iyi model ![image](https://github.com/user-attachments/assets/6a775398-9698-4e4a-96c0-beff19844aba)

%97 ile Lojistik Regresyon oldu.Hiperparametre optimizasyonu,Test verisi üzerinde tahmin ve değerlendirme,sınıflandırma raporu ve confusion matrix ile işlemlerimi tamamlamış oldum.

# Metrikler
Bu proje kapsamında tüketici ürün yorumlarını analiz ederek, yorumların olumlu mu olumsuz mu olduğunu sınıflandırmayı hedefledim. Supervised Learning (Gözetimli Öğrenme) yöntemleriyle çeşitli algoritmalar denedim ve Logistic Regression modelinin en iyi sonucu verdiğini gözlemledim.

Modelin değerlendirme metrikleri şu şekildeydi:

Doğruluk (Accuracy): 0.968
Kesinlik (Precision): 0.965
Duyarlılık (Recall): 0.968

F1 Skoru: 0.966

Bu sonuçlar, modelin hem olumlu hem de olumsuz yorumları yüksek doğrulukla tahmin edebildiğini gösteriyor. F1 Skoru’nun yüksek olması, modelin hem hassas (precision) hem de duyarlı (recall) olduğunu, yani dengesiz veri kümelerinde dahi başarılı sonuçlar verdiğini ortaya koyuyor.

 Ayrıca, Grid Search ile hiperparametre optimizasyonu uygulayarak modelin performansını artırmaya çalıştım. Bu optimizasyon sonucunda doğruluk oranında küçük ama anlamlı bir artış gözlemledim.

 Karışıklık matrisi sayesinde hangi sınıflarda modelin hata yaptığını daha iyi görebildim. Bu matrise göre model, çoğunlukla doğru tahminlerde bulunsa da bazı azınlık sınıfları karıştırabiliyor. Bu da gelecekte sınıf dengesini iyileştirme ya da veri artırma (data augmentation) gibi yöntemleri değerlendirmem gerektiğini gösteriyor.



# Link
https://www.kaggle.com/code/melihtalhaelik/machine-learning-supervised-project/edit
