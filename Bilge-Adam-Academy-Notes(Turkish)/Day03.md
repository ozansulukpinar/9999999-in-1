## C# Introduction

15 Şubat 2019

- Yorum satırı eklemek için kısayol: Ctrl+K+C
- Yorum satırını kaldırmak için kısayol: Ctrl+K+U

### Output İşlemleri

**Console.Write():** Ekrana bir mesaj yazdırmak için kullanılır. Write komutundan sonra yazı yazma imleci mesajın yanında yanıp söner ve bir alt satıra inmez.
**Console.WriteLine():** Ekrana bir mesaj yazdırmak için kullanılır. Write komutundan sonra yazı yazma imleci bir alt satırda yanıp söner.

### Input İşlemleri

**Console.ReadLine():** Bulunduğu satırda kullanıcının giriş yapmış olduğu veriyi okuma işlemi yapar, aynı zamanda enter tuşuna basılana kadar programın açık kalmasını sağlar.
**Console.ReadKey():** Bulunduğu satırda kullanıcının giriş yapmış olduğu veriyi okuma işlemi yapar, aynı zamanda herhangi bir tuşa basılana kadar programın açık kalmasını sağlar.

### Tip Dönüşümleri

**Parse():** string tipteki verilerin sayısal tiplre dönüşümünü sağlayan metottur.
**ToString():** Bir değişkenin string veri tipine dönüştürmek için kullanılan metottur.
**Camel case:** Kelimeler bitişik, ilk kelimenin hepsi küçük, bir sonraki kelimelerin baş harfleri büyük olacak şekilde yazım stilidir.
**Pascal case:** Değişken, sınıf metot veya fonksiyon isimleri kelimeler bitişik ve baş harfler büyük şekilde yazım stilidir.
**Reserved keywords:** C# derleyicisinde tanımlı özel kelimelerdir, kod sayfasında mavi renkte (mavinin tonları) olarak görünür.
Console ekranını cash'te kalmasını engellemek için solution üzerinde sağ tık clean solution yapabilirsiniz.

### Operatörler

#### Mantıksal Operatörler

#### Karşılaştırma Operatörleri

**&(ve):** Her iki şart da sağlanıyorsa true sonucu döner, iki şarttan bir tanesi sağlanıyor bir tanesi sağlanmmıyorsa false döner.
**||(veya):** Şartlardan bir tanesi sağlandığından true döner, iki şart da sağlanmazsa false döner, diğer ihtimallerde true döner.
**!(değil-not):** İşlemin tersini almak için kullanılır.

#### İlişkisel Operatörler

            >(büyüktür)
            <(küçüktür)
            <=(küçük eşit)
            >=(büyük eşit)
            ==(eşittir)
            !=(eşit değildir)

#### Matematiksel Operatörler

            +(toplama)
            -(çıkarma)
            *(çarpma)
            /(bölme)
            %(mod alma)

            +=(toplayarak ekle)
            *=(çarparak ekle)
            /=(bölerek ekle)
            -=(çıkararak ekle)

### Değişkenler

**Değişken:** Verilerin geçici olarak depolandığı yer.

#### Değişken Kuralları

Veri tipi uyumluluğu
_ değişken adı sayı ile başlayamaz.
_ kullanmayacağınız değişkeni tanımlamayın.
_ türkçe karakter kullanılması tavsiye edilmez.
_ değişken tanımlanırken boşluk bırakılmaz, gerekirse \_ ya da camelCase yazım kullanılabilir.
_ kullanılacak veriye göre değer aralığı seçmek gerekir(performans yönetimine katkı).
_ aynı değişken adı birden fazla kere kullanılmamalı. \* kod ifade eden kelimeler değişken adı olarak kullanılmaz.

##### Metinsel Veri Tipleri

**string:** İçinde tüm metinsel ifadeleri, tek karakter verileri tutabilen veri tipidir. İçinde sınırsız veri tutar, 2 gb'a kadar yer kaplayabilir.
**char:** İçinde tek karakter barındıran veri tipidir, 16bit, unicode karakter.

##### Mantıksal Veri Tipi

**bool:** true ya da false değerini içinde tutar.

##### Tarih Veri Tipi

İçinde zaman bulunduran veri tipidir.
