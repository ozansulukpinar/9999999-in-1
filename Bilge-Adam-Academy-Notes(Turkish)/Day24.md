## OOP Introduction

18 Mart 2019

Instance alarak örnek sınıftan yeni bir nesne oluşturulur.

### ACCESS MODIFIERS (ERİŞİM BELİRLEYİCİLER)

**private:** En düşük seviye erişim belirleyicisidir. Sınıfın üyelerinde kullanılır, yalnızca o sınıf üyeleri tarafından erişilebilir. Bu üye metot ya da değişken olabilir. Yani o üyenin o tipe(sınıfa) özel olmasını sağlar. Private üyeler kalıtım yoluyla yaratılan sınıflardan bile erişemez. Eğer üyelere herhangi bir erişim belirleyici atanmazsa o üye derleyici tarafündan private olarak algılanır. Yani üyelerin varsayılan (default) erişim düzeyi private'dır.

**protected:** Bu erişim belirleyicisi ile tanımlanmış üyeler (field,metot,...), kalıtım alınarak oluşturulmuş sınıflardan da erişilebilir. Örneğin, vasıta sınıfı oluştururken tanımlanmış protected bir üye, vasıtadan kalıtım alınarak oluşturulmuş gemi isimli sınıftan erişilebilir(private olsaydı erişilemezdi.).

**internal:** Dahili anlamına gelmektedir. Yalnızca bulunduğu assembly'den erişilebilir. Burada assembly'den kastedilen projenin kendisidir. Yani, bir kütüphane, namespace(.dll) oluşturursanız, internal bir sınıfa sadece o kütüphaneden erişebilirsiniz. Internal, sınıf üyeleri için de kullanılabilir, aynı etkisi vardır. Bir sınıfın erişim belirleyici tanımlanmamışsa varsayılanı internal'dır.

**protected internal:** Erişim yapılan yere göre internal ya da protected davranır. Doğal olarak assembly dışından erişilmeye çalışıldığında internal, aynı assembly'den erişilmeye çalışıldığında protected davranış gösterir.

**public:** En sınırsız erişim belirleyicisidir. Hem sınıf hem üyeleri için kullanılabilir. İkisi için farklı anlamları vardır. Örneğin bir sınıf public ise o sınıf bulunduğu assembly dışından dahi erişilebilir. Sınıfın üyeleri için public ise o üyeye de her yerden erişilebileceği anlamına gelir. Doğal olarak bu sınıftan kalıtım yoluyla üretilen bir sınıf varsa onlardan da dahi erişilebilir.

**Reference Type:** string, object, array, class
**Value(Değer) Type:** int, double, bool, byte, char ("null" olamazlar).

**Boxing:** Value type'ın bilinçsiz olarak reference type'a dönüşümüdür.
**Unboxing:** Reference type'ın value type'a bilinçli dönüştürülmesi.

#### Inheritence

Bir sınıf sadece bir sınıftan kalıtım alabilir. Multiple inheritance yoktur.
