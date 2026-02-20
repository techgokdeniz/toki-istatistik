# TOKİ 500.000 Konut - Talep Analizi

[talep.toki.gov.tr](https://talep.toki.gov.tr/500binkonut/) adresindeki kamuya açık veriler kullanılarak 81 il için kategori bazlı kazanma şanslarını hesaplayan bir analiz.

**[index.html](index.html)** dosyasını tarayıcıda açarak sonuçları görüntüleyebilirsiniz. Sunucu veya kurulum gerektirmez.

## Nasıl Yaptım

1. TOKİ'nin talep sayfasından 81 ilin proje verilerini çektim (il, ilçe, konut sayısı, kabul listesi linkleri)
2. Her proje için kabul listesi PDF'lerini indirdim (~857 PDF)
3. PDF'leri parse ederek kategori bazlı başvuru sayılarını çıkardım (Genç, Emekli, Engelli, 3+ Çocuklu, Şehit/Gazi, Diğer)
4. TOKİ'nin kontenjan oranlarına göre (%20 Genç, %20 Emekli, %5 Engelli, %10 3+ Çocuk, %5 Şehit/Gazi, %40 Diğer) her kategori için kazanma şansını hesapladım
5. Bir kategoride başvuru kontenjandan az ise fazlayı Diğer'e aktardım
6. Tüm veriyi tek bir self-contained HTML dashboard'a gömdüm

## İletişim

- [gokdeniz.dev](https://gokdeniz.dev/)
- [LinkedIn](https://www.linkedin.com/in/gokdeniz/)
- [X (Twitter)](https://x.com/gokveyadeniz)
