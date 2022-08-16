## HTML

13 Mayıs 2019

### Table(Tablo)

- **tr:** table row
- **td:** table data
- **th:** table head: td elementinden farkı otomatik olarak bold ve ortalanmış olur.

### Listeler

**ordered list:** numaralanmış liste, <ol></ol>
**unordered list:** sırasız liste, <ul></ul>

**HTML(Hyper Text Markup Language):** HTML kodları sayfanın iskeletini oluşturduğumuz kısımdır, bu kodlar tarayıcı tarafında yorumlanarak çalışır(HTML bir programlama dili değildir, işaretleme dilidir.).
**Server Side(Sunucu):** Sunucular web sitesine ait dosyaları barındırır ve bu dosyaları internette paylaşmayı sağlar. Programlama dillerini okuyup çalıştırabilir. Kullanıcıdan gelen isteklere göre işlemleri gerçekleştirip sonuç verirler ve gerekirse yeniden işlem yaparlar.
**Client Side(İstemci/Kullanıcı):** Sunuculara dosyaları açması ve belli işlemleri gerçekleştirmesi için HTTP ve HTTPS protokolleri üzerinden istek gönderen kullanıcı ya da istemcidir.
Öncelikle kullanıcı istekte bulunur, sunucu işlemi gerçekleştirmeye başlar, eğer dosyayı bulursa sonucu 200(başarılı) olarak döndürür. Bu cevap sayfanın bulunduğu ve yüklenmekte olduğu anlamına gelir. Bunun gibi farklı HTTP Request kodları vardır.

### Request(istek)&Response(cevap)

Request post metodunu => head+body içinde kullanabiliriz.
Request get metodunu => head içinde kullanabiliriz.

**DNS(Domain Name Server):** IP adreslerinin karşılığı olan isimlerini tutar. Kullanıcı Request'te bulunduğunda önce DNS üzerinden istekteki adres tespit edilir daha sonra o adresin IP numarası Server'a gider.

```html
<hr />
<!-- Çizgi çekmek için kullanılır. -->
<b></b>
<!-- Yazıyı vurgular. -->
<strong></strong>
<!-- Yazıyı vurgular. -->
<i></i>
<!-- Yazıyı italik yapar. -->
<em></em>
<!-- Yazıyı italik yapar. -->
<u></u>
<!-- Yazının altını çizer. -->
<ins></ins>
<!-- Yazının altını çizer. -->
<p></p>
<!-- Paragraf etiketidir. -->
<span></span>
<!-- İçindeki veri kadar yer kaplar. -->
<br />
<!-- Bir alt satıra geçer. -->

<input type="checkbox" />
<!-- Tıkla -->
<input type="button" />
<!-- Click'ini kendimiz açıp yazmalıyız. -->
<input type="submit" />
<!-- Click'i halihazırda yazılıdır. -->
<input type="email" />
<!-- Email giriniz.. -->
```
