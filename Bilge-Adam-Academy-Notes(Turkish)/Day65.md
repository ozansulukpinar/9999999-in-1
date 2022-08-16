## JavaScript

16 Mayıs 2019

**JavaScript:** HTML sayfalara etkileşim eklemek için tasarlanmıştır. Javascript ile neler yapılabilir:

- HTML sayfalarına dinamik metin eklenebilir.
- Olaylara karşılık verebilir.
- HTML öğelerini okuyabilir ve onlarla ilgili işlem yapabilir.

Head etiketinin içine yazılan JS kodları sayfa ilk çağrıldığında çalışır. Body etiketinin içine yazılan JS kodları sayfa ilk yüklenirken çalışır.

Script içinde elementleri nesne gibi yakalıyoruz. Fakat kodu yorumlayıcı yukarıdan aşağıya doğru okuduğundan yakalama sırasında ilgili nesne henüz oluşmamış ise hata alırız. Bunun için JS kodlarını yazdığımız yer önemlidir.

### Değişkenler

**let:** let ile bu isimde bir şey tanımladıktan sonra o isimle bir daha bir şey tanımlayamayız.
**alert():** alert bütün her şeyi ezip sayfaya ilk çıkar.

alert output için kullanılır. GUI(Graphical User Interface)'yu durdurur, arka planda kodlar çalışsa da GUI durdurulduğu için görseller alınamaz.

**prompt:** ileti kutusu, kullanıcıdan veri almak için kullanılır.
**confirm:** onay kutusu, kullanıcıdan mesaj vererek onay almayı sağlar.

İç içe tırnak kullanırken hangisiyle başladıysam diğeriyle devam etmeliyiz. Console ekranına mesaj yazdırmak için kullanılır. Text-kontrol ya da yazılımcıya mesaj bırakmak için kullanılır. User görmez.

**isNaN():** Mantık olarak tersten yaklaşır, sayı girişi yapıldığında false kullanılır.Metodun aldığı değerin/değişkenin rakam olup olmadığını kontrol eder. Eğer rakam değilse (NaN-not a number) true döndürür. Diğer türlü false döndürür.

### Karşılaştırma Operatörleri

**==:** Sadece değer kümelerine bakar, tipe bakmaz.
**===:** Hem tip olarak hem de içerik olarak aynı olmalı, tipli karşılaştırma, katı eşitlilik.

### Mantıksal Operatörler

**&&:** İçeriğindeki her koşulu kontrol etmez, ilk koşulda false değeri alırsa diğerlerine bakmaz. Diğer koşulları çalıştırmadan atlar.
**||:** İçeriğinde herhangi bir koşul true olduğunda sonrakilere bakmaz. Diğer koşulları çalıştırmadan atlar.
**&:** Herhangi karşılaştırma false verse de tüm karşılaştırmalar çalışır.
**|:** Herhangi karşılaştırma true verse de tüm karşılaştırma çalışır.

### Fonksiyonlar

```js
// Obje içinde fonksiyon kullanımı
var insan = new Object();
insan.ad = "Ozan";
insan.Konus = function () {
  return "konuşuyor";
};

// Prototype üzerinden fonksiyon ekleme
Date.prototype.Ayiver = function () {
  var ayIndis = this.getMonth();
  return ayIndis + 1;
};
```
