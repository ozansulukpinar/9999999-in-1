## Tip Dönüşümleri

18 Şubat 2019

Karar Yapıları
Uygulamalarımızın çalışması esnasında farklı senaryolara göre farklı yönlendirmeler yapabilmek için kullanılır.
Üç temel karar yapısı vardır.
_ If-Else
_ Switch-Case \* Ternary-If
Random(): Random sınıfından instance alarak yani bir kopyaını oluşturarak rastgele sayı üretmek için kullanırız.

Tip Dönüşümleri
Cast(Maskeleme): Değişken aynı değişkendir, sadece maskeleyerek tipini değiştirmiş oluruz yani farklı şekilde göstermiş oluruz.

Dönüşüm yapmak istediğinizde eğer cast imdadınıza yetişmiyorsa o zaman başka bir dönüşüm yöntemi olan Convert işlemini kulanabiliriz.

Convert: Convert işlemi gerçek bir çevirme işlemidir, ham veriyi eski değerinden kopartıp çevirme işlemi yapılır

Cast ve convert hangisini kullanacağıma nasıl karar vereceğim:

- Eğer büyük bir veriyi küçük bir veriye çevireceksem convert kullanmam lazım, örneğin integer-byte dönüşümü yapacaksam bunu cast ile yaparsam byte'a sığmayan kısımlarda veri kaybına uğrarım bu yüzden convert kullanmam gerekir.
- Cast ile küçük bir veriyi büyük veri tipine çevirirken ör:byte-integer, integer zaten byte'ın tamamını kapsar bu yüzden sorun çıkmaz.
- Int32.Parse() veya Int.Parse() ikisi de int türüne çevirir, yani Converty.ToInt32 fonksiyonu ile aynı işleve sahiptir.

- Int32.Parse() fonksiyonuna parametre olarak null değere sahip veri girerseniz "ArgumentNullException" hatası verir.
- Convert.ToInt32() fonksiyonunda 0(sıfır) değerini verir, yani hata vermek yerine sıfır değerini döndürür.
- Convert il virgüllü bir sayıyı tam sayıya çevirmek istediğimizde virgülden sonraki değer 5 ve 5'ten büyükse yukarı, 5'ten küçüks aşağı yuvarlar.

Try Catch Hata Denetimi
İstisna Tipler

- Çalışma zamanı hataları(Runtime Exception): Çoğunlukla kullanıcı kaynaklı hatalardır(verinin eksik ya da yanlış girilmesi, boş geçilmesi) Çözüm yolu olarak try-catch işe yarar.
- Derleme zamanı hataları(Compile Exception): Tamamen yazılımcı kaynklıdır, yazım hataları meydan geldiğinde olur, çözümü en kolay olan, visual studio sizi uyarır(error list) penceresi, hatayı çift tıklayarak ayrıntısına ulaşıp sebep olan işlemleri görüp düzeltebiliriz.
- Mantıksal hatalar: Tamamen programcı kaynaklı, uygulamanın algoritmasında meydan gelir, örneğin bölme yapılacak yerde işlemin unutulması, değerin yanlış bir değerle değiştirilmesi...Çözümü en zor hatalardır.Anlık olarak derleme esnasında takip edilmeli ve hatayı görüp düzeltilmelidir.

Breakpoint, watch penceresi gibi tool'lar işimizi kolaylaştırır.

Breakpoint: Derleme aşamasında adım adım dahil olmak için kullandığımız tool'dur. İlgili satırın sol kısmındaki gri alana tıklayarak kırmızı bir nokta koyarız, daha sonra debug edip F10 ile adım adım kodları takip ederiz. Değişkenlerin içindeki değerleri, kodların akışını detaylı bir şekilde görebiliriz.

Watch penceresi: Yalnızca runtime'da kullanılabilir, program çalışırken debug-windows-watch şeklinde ulaşılır, noktalar, virgüller yazım syntax'ı watch penceresi içerisinde geçerlidir.

Not: Eğer dışarıdan bir veri girişi varsa ve tutarlılığından emin değilseniz orada hata riski vardır ve try-catch kullanılmaı gerekir.

            /*
             try
             {
             //bu alana riskli kodlar yazılır
             }
             catch
             {
             //try bloğu içerisine yazılan kodlarda herhangi bir hata meydana gelirse buradaki kodlar çalışır
             }
             finally
             {
             //hata olsa da olmasa da çalışmasını istediğimiz kodları yazdığımız alan(opsiyoneldir)

//Kullanılmasa da olur try bloğunun son adresidir. Genelde temizleme işlemleri databe bağlantısının RAM'den düşürülmesi gibi işlemlerde kullanılır.
}
\*/
