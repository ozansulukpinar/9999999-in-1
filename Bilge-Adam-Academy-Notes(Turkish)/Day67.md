## Jquery

20 Mayıs 2019

**jQuery:** Az kodla çok iş yapar.
Kütüphanesi şu özellikleri içerir:

- HTML/DOM(Document Object Model)
- HTML olay metodları
- Efektler ve animasyonlar

**CDN(Content Delivery Network, İçerik Dağıtım Ağı):** Statik içeriklerinizin normalden daha hızlı tarayıcıya ulaştırılması için düşünülmüş bir dağıtım yapısıdır.

### Selectors(Seçiciler)

```js
$("p.note");
$("p#note");
$("p");
$("input[name='test']"); //name'i test olan bütün input'ları yakalar
$(this); //this'in içindeki geçtiği elementi yakalar
$("p>a"); //p'nin içindeki a'lar
$("p:first"); //ilk p'yi getirir
$("p:has(a)"); //içinde a olan bütün p'ler
$("*"); //tüm elementleri yakalar
$("#ozan"); //ozan id'li elementleri yakalar
$(".aziz"); //aziz class'lı elementleri yakalar
$("#ali .sil"); //ali id'li sil class'lı olanları yakalar
$("#cansu>a"); //cansu'nun çocuğu olan a'ları yakalar
$(".yasin:first"); //yasin class'ına sahip olan ilk elementi yakalar
$("div[name='umut']"); //name'i umut olan div'leri yakalar
$("div[class$='oglu']"); //sonunda oglu geçen class'lar
$("div[class^='oglu']"); //başında oglu geçen class'lar
$("div[class~='oglu']"); //içinde oglu geçen class'lar
$("div[class*='oglu']"); //içinde geçenleri her türlü alır
$(".mahmut:first-child"); //mahmut sınıfındaki ilk çocuğu yakalar
$(".suheda+label"); //şüheda class'ından sonraki ilk label
$("div>a:first-of-type"); //div'in içindeki ilk a tipindeki element
$("a:parent"); //bütün a elementlerinin bütün babalarını yakalar
$("a:hidden"); //saklı olan a elemanlarını yakalar
$("a:eq(3)"); //document'te üçüncü indise sahip a (indis'ler 0'dan başlar)
$("a:odd"); //document'te indisi tek olanlar
$("a:even"); //document'te indisi çift olanlar
$("a:nth-of-type(3n+3)"); //eq özel hali, indis alıri even ve odd alır, formül alır
jQuery(".aClass").css({ "font-size": "25px" }); //$ işareti yerine jQuery de yazabiliriz.
```

### Hazır Metotlar

```js
$(".kutu").show();
$(".kutu").toggle();
$(".kutu:odd").fadeOut(4000);
$(".kutu:odd").fadeIn(3000);
$(".kutu").slideUp();
$(".kutu").slideDown();
$(".kutu").slideToggle();
```

### Event

```js
jQuery.noConflict();
```

Kimlik belirleyici ($) simgesi kaldırılır. İstediğimiz herhangi bir ifadeyi kimlik belirleyici olarak atayabiliriz, burada $ ya da jQuery yerine artık $$ kullanacağımızı belirtmiş oluruz.

```js
        .on() //buraya istediğimiz kadar event yazabiliyoruz.
        $("ul").html("<li>bir öge</li>");
        $("ul").append("<li>append</li>"); //en son append'dakini ekler.
        $("ul li:first").before("<li>before</li>"); //ilgiliden bir önce ekler.
        $("ul li:nth-of-type(1)").after("<li>after</li>"); //ilgiliden bir sonra ekler.
        $("ul li:nth-of-type(5)").remove(); //indisi 1'den başlar.
        $("ul li:even(2)").remove(); //indisi 0'dan başlar.
        $("ul").empty();

        parent():baba olanı getirir.
        Sibling():kardeşleri getirir.
        Children():çocukları getirir.
        Find():ilgili alanda selector ile arama yaptırır.
        End():bir önceki elemente dönüş yapılır.
```

**Ajax(Asynchronous Javascript and XML, Eşzamansız JS ve XML):** Bütün sayfayı kullanıcıya tekrar yükletmeden, sadece gerekli olan veriyi dinamik olarak ekrana getirmek ve ya sunucuya veri göndermektir. Örneğin iletişim formu doldurduğumuzda sadece detayı göndererek o bölüme sonucu yazdırmak için kullanılabilir.

**Bootstrap:** Açık kaynak kodlu ve ücretsiz bir CSS framework'dür.
Neden Bootstrap kullanmalıyız:
Bootstrap sayesinde masaüstü, tablet, mobil cihaz ve tüm tarayıcılara uyumlu web siteleri geliştirebiliriz.
Bootstrap bir web sitesi için gerekli olan tüm bileşenleri barındırır; formlar, tablolar, butonlar, uyarılar, menüler, sayfalandırma vs.
Zamandan tasarruf, özelleştirilebilir, tutarlılık(bütün platformlarda aynı sonuçları verir), gelişmeye devam ediyor, entegrasyonu kolay (kolay ve hızlı), responsive, geleceğe uyumlu, dökümantasyonu var.

Bootstrap yatayda 12 pikseldir ancak customize edilip değiştirilebilir.
jQuery'nin olup olmadığını sitede F12'ye gidip Console kısmına Jquery yazarız, kırmızı hata almıyorsak jQuery ekli demektir.
**const-container:** Sayfa genişliğinde ortalar.
**container-fluid:** Tüm sayfa genişliğini kullanır.

Grid ekran modelleri;

- telefon: col(extra small)
- tablet: col-sm(small)
- dizüstü bilgisayar: col-md(medium)
- masaüstü bilgisayar: col-lg(large)
- televizyon: col-xl(extra large)

**Keexbox:** Kendine ait class'ları olan esnek kutulardır.
**justify-content-around:** aralıklarla sayfaya yayar, ortaya doğru.
**justify-content-end:** ortalar.
**justify-content-between:** sayfayı kenarlara doğru aralıklarla yayar.

href'e yazdığım id ile aynı sayfa içerisinde ilgili kısma gönderebiliyorum.
