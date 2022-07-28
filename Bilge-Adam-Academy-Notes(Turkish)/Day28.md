## OOP

22 Mart 2019

Bir sınıftaki öğeler ya static ya da non-static (nesnenin üyesi) olabilir. static öğeler sınıfın ismiyle çağrılır, non-static olanlar nesnenin ismiyle çağrılır. static üyeler program çalıştığı anda RAM'e çıkarılır ve istenildiği zaman kullanılabilir. static işaretlenebilecek sınıf üyeleri : field, property, method, constructor. static ctor'lar sınıf içindeki static field'ları initialize etmek için kullanılır. O sınıftan ilk instance alındığında static ctor sadece bir kereliğine çalışacaktır.
static Değişken : Bu değişken RAM'e sadece bir kere çıkarılır. Tekrar tekrar instance alındığında bu değer sabit kalır ve o değer üzerinden işlem yapabilirim. Eğer değişken static değil ise static metot'tan ona erişemem. Çünkü metot RAM'e bir kere çıkıyor ancak değişken her nesne için başka başka olabilir. Ama eğer değişken static ise static metodun içerisinde erişip kullanabiliyorum.
Main() metodu static bir metottur. O yüzden main dışında tanımladığım metotları, main metodu içerisinde kullanabilmem için o metotların da static olması gerekiyor.

Static Sınıf
static sınıflar içerisinde sadece static üye tanımlamaları yapabiliriz. static sınıftan nesne oluşturamayız, instance alamayız. static olarak işaretlenen bir sınıf proje çalıştırdığında RAM üzerine çıkarılır. static constructor'a access modifier verilemez. Normalde sınıf üyeleri her oluşturulan nesneye(this) ait olduğu için static bir sınıfta böyle bir tanımlama yapılamaz.
static olan sınıftan instance alamam(?)

field'lar içim readonly keyword'unu kullanarak onu sadece okunabilir kılarız.
const sabit demektir. Sadece okuyabiliriz, değer atamayız. Non-static sınıflarda da kullanılabilir.\*const üyeler otomatik olarak static'tir.
static class içinde readonly field'a sadece static ctor'dan değer atayabilirim.
property'nin sadece get accessor'u olduğunda okuyabiliyor, set işlemi yapılamıyor.
field readonly olduğu için sadece okuyabilinir ve sadece kendi ctor'undan değer atanabilir.

Guid g = new Guid(): struct olduğu için instance aldım.
g = Guid.NewGuid(): Kendisi static olmasa da NewGuid metodu static bir metot olduğundan nesneden değil de sınıfın kendisinden o metodu çağrılır.

Delegate (delege, temsilci, function pointer) : Metot işaret eden yapılardır. Temel tiplerden birisidir. Reference type'dır. İçerisinde metotların bellekteki adreslerini tutarlar ve olay güdümlü yapılarda kullanılırlar. Genellikle isimlendirilirken sonuna Handler ifadesi eklenir. Delegate'ler tutacakları metotla aynı dönüş tipine sahip olmalıdırlar. delegate'i kullanmak için instance almak gerekir.
Delegate nesne invoke edildiğinde işaret ettiği tüm metotları eklenme sırasına göre çalıştırır. Delegenin geri dönüş tipi parametreleri de metotla aynı olmalıdır(metot imzası).

Event: Delegeyle beraber çalışacak evet delege'nin tipinde olmalıdır.
