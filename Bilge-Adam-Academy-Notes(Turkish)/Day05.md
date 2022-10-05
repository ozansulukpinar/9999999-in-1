## Switch-Case

19 Şubat 2019

### Hata Yönetimi

**Exception Handling (Hata yönetimi):** Yazılım geliştirirken farklı tiplerde birçok hata ile karşılabiliriz. Bir hata ile karşılaştığımızda bu hataların öncelikle ne tür bir hata olduğunu bilmemiz gerekmektedir. Hatalar kendi içerisinde gruplara ayrılır:

**Syntax Errors (Derleme Zamanı Hatası):** Syntax hataları, bir yazılımcının en çok karşılaştığı hata çeşididir. Hatayı bulmak ve yönetmek kolaydır. Error list penceresinde hata mesajı görünür. Syntax hatalarını düzeltemezsek program çalışmayacaktır.

**Runtime Errors (Çalışma Zamanı Hatası):** Programda syntax hatası olmamasına karşın kullanıcının yanlış bilgi girmesi veya programcının kontrol altına almadığı bir durum sonucu ortaya çıkan hatalardır. Bu tür hataları önlemek için kullanılan yapılar bulunmaktadır(try-catch-finally).

```csharp
            try
            {
            }
            catch (FormatException hata) // Format hatası olduğunda yakalar
            {
                Console.WriteLine("Lütfen doğru formatta veri giriniz.\n" + hata.Message);
            }
            catch (DivideByZeroException hata)
            {
                Console.WriteLine("Sıfıra bölünme hatası. Sayı sıfıra bölünemez.\n" + hata.Message);
            }
            catch (OverflowException hata)
            {
                Console.WriteLine("Değişken sınırları dışına çıktınız.\n" + hata.Message);
            }
            catch (Exception hata)
            {
                Console.WriteLine("Başka türde bir hata \n" + hata.Message);
            }
```

**Logical Errors (Mantıksal Hatlar):** Tespit edilmesi en zor hata çeşididir. Üstte belirttiğimiz hatalar gibi programda bozukluğa sebep olmaz. Yazdığımız kodlar istediğimiz sonucu dönmüyorsa mantıksal bir hata ile karşı karşıya olabiliriz. Mantıksal hataları tespit etmek için Runtime esnasında adım adım kontrol etmemiz gerekebilir.

**Breakpoint (Duraklama Noktası):** Debug işlemi sırasında kod akışını takip edebilmemizi sağlayan özelliktir. Proje çalışırken anlık olarak izlememize olanak sağlar.
**F10:** Kod akışını takip etmeksizin izlemeye alır. Her tıkladığımızda satır satır kod akışı ilerleyecektir.
**F11:** Kod akışını takip ederek izlemeye alır. Uygulamadaki kod akışını takip ederken, kod akışı farklı bir event ya da methoda yöneliyorsa kod akışını orada da izlemeye devam eder.

### Nullable Tipler

C#'ta tipler iki kategoride ayrılır:

**Value Types:** int, float, double vs.
**Reference Types:** string, sınıflar, diziler vs.

Default olarak value type'lar null değer alamazlar.

```csharp
int? i = null; // Artık i değişkenim nullable-int
```
