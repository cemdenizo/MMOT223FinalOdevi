# MNOT223 Final Ödevi Dökümantasyonu
## Grup Üyeleri:
![ekip](https://drive.google.com/uc?export=view&id=1FbO1EvGYAAAvNWumVvaYAbtoCQ_uLVdO)
## Ödev Konusu:
#### Proje kapsamında oluşturulan ML.NET projesi  referans alınarak "WEB, Windows Form yada Console" uygulamasından biri üzerinden proje uygun bir arayüzle modellenecektir Proje kapsamında kodlarınız Github üzerinden yayınlacak ve github linki Olearn den teslim edilecektir Proje içinde readme.md dosyası yer alacak içinde proje mimarisi, dosya yapısı ve kapsamı özetlenecektir
## Orjinal Dataset
https://www.kaggle.com/irkaal/english-premier-league-results/code
https://github.com/burakodaloglu/Dataset
## Kullanılan Dataset
https://drive.google.com/uc?export=view&id=1WKGv_FbzXpRtXXB3Tsg33K2eocUr0e4d
## Dataset Tanımı
- HomeTeam = ev sahibi takım
- AwayTeam	= rakip takım
- FTHomeGol	= maç sonu ev sahibi gol sayısı
- FTAwayGol = maç sonu rakip gol sayısı
- HomeShot = ev sahibi şut sayısı
- AwayShot = rakip şut sayısı
- HomeCorner = ev sahibi korner atışı sayısı
- AwayCorner = rakip korner atışı sayısı
## ML.NET Kullanımı
ML.NET "Value Prediction" senaryosu kullanıldı. HomeShot Column to predict olarak seçildi. Modelin tahmin gücü olan RSquared ölçüsü 0.42 olarak çıktı.
ML.NET "Value Prediction" senaryosu kullanıldı. HomeShot, "Column to predict" olarak seçildi. Modelin tahmin gücü olan RSquared ölçüsü **0.42** olarak çıktı. Farklı sütun seçildiğinde tahmin gücü daha düşük çıktı.
## Model Consumption
ML.NET in oluşturduğu modeli Visual Studio 2019 ile **ASP.NET Core Web Application**(Model-View-Controller) kullanarak çalışır hale getirdik. Ayrıca **Microsoft IIS(Internet Information Services)** kullanılarak bir web sunucusu yaratılmıştır.
## Gelişme Alanları
- Modelin RSquare ölçüsü arttırılmalı -> Dataset geliştirilmeli
- Farklı ülkelerin lig dataları ile modeli "train" edilmeli
## Kaynak
https://www.c-sharpcorner.com/article/price-prediction-in-asp-net-core-using-ml-net/