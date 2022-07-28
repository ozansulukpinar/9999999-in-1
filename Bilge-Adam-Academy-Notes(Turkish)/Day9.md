## Metotlar

25 Şubat 2019

Metotlar
Method overload: Aynı isme sahip birden fazla metot olabilmesidir diyebiliriz. Kural olarak overload edilmiş metotlar aynı metot imzasına (signature) sahip olamazlar. Metot imzası metodun ismi ve aldığı parametrelerin tipleri adetleri vs.dir. Metot imzasına dönüş tipi dahil değildir.

out parametresi : Metot içerisinden dışarıya birden fazla değer çıkarmamızı sağlar. out anahtar kelimesi metoda gönderdiğimiz parametre değişkeninin referanını gösterir.
ref parametresi : Normal metotlar içerisine parametre üzerinden gönderilen değerin bir kopyasını oluşturarak işlemleri oluşturulan kopya üzerinden yapar. ref parametresi kullanıldığında, gönderilecek değişkenin kopyasını oluşturmak yerine, referans adresini göndererek, verinin kendisi üzerinden işlem yapar.
param parametresi: Metotlara parametre gönderirken parametre sayısını bilmediğimiz durumlarda kullanılır. metot içeirisine aynı tipte sınırsız değer gönderilebilmesini sağlar.

Bir metotta birden fazla param kullanılamaz. params anahtar kelimesi metodun son parametresinde kullanılmalıdır.
