## Design Pattern

30 Mayıs 2019

**Design Pattern:** Prensipleri uygulayan standartlaşmış çözümlerdir, design pattern aslında bir şablondur. Design Pattern uluslararasıdır.
Örneğin; bir yazılım ekibi var ve bir proje geliştiriyorlar, ekibe yeni biri katıldığında eğer geliştirilen projede bir design pattern kullanıldıysa ekibe yeni katılan kişinin kodları okuması daha kolay olur.
Gang of Four isimli dört kişiden oluşan bir ekibin bir kitap çıkarması ile Design Pattern ortaya çıkmıştır. Bu kitapta 24 tane Design Pattern'dan bahsedilmiş ve üç grupta incelenmiştir:

- Creational Pattern(yaratıcı)
- Structural Pattern(yapısal)
- Behavioral Pattern(davranışsal)

Martin Fowler abimiz Enterprise Design Pattern kitabında 51 tane Design Pattern'dan bahsetmiştir ve bunlar katmanlı mimarideki katmanlarla ilgilidir.
MVC'de bir pattern'dir.

## Singleton Pattern

constructor private ile gizlendiği için bir daha instance alımına izin vermez.
Nesnenin sadece tek bir instance'ının alınması için kullanılan pattern'dir, gereksiz instance alınma ihtimalini ortadan kaldırmak için kullanılır.
Çoklu istemcili, örneğin bir web projesindeki nesne için singleton uygulayacaksak oluşturulan ilk örneğin kilitlenmesi gerekir. Eğer kilitleme yapılmazsa iki farklı thread art arda yapacağı istek sonucu, birinin sonucuna ulaşamadan yeni bir örneklendirme yapar. Kilitleme yapılırsa nesne örneği kilitli olacağından, oluşturulan ilk örneğin bitmesini bekler ve ikinci bir istek yapıldığında oluşturulan ilk örneği kullanır.

**Load Balancer(Yük Dengeleyici):** Gelen isteği(request) sunuculardan yükü az olana yönlendirir.

Trafikte akış sunucuların önüne konan bir yük dağıtıcı ile karşılanarak eşit oranda(veya belirli kurallara göre) asıl işi yapacak olan sunucuya dağıtılır.
Problemli ya da yoğun olan sunucuya istek gönderilmez ve kullanıcıların problemden etkilenmemesi sağlanır, load balancer sayesinde uygulama güncellemeleri sistemde kesintiye sebep olmadan yapılabilir.

Factory'ler gruplanacaksa abstract factory kullanılır. Factory'nin de factory'sidir(fabrikanın fabrikası).

### Factory Pattern(Fabrika)

Seçime göre nesne oluşturmak için kullanılır, işin içinde interface ya da base class vardır.
Aynı interface'i ya da abstract sınıfı implement etmiş factory nesnelerinin üretiminden sorumlu pattern'dır.
Teknik tanıma göre, aynı abstract veya interface'den türeyen nesnelerin üretiminden sorumlu yapıdır, bu pattern ile nesne yaratılma işini inheritance yoluyla client-side'dan ayırıp sub-class'lara vermek amaçlanır.
Gang of Four pattern'ları günümüzde en sıkı şekilde takip edilen ve en çok kullanılan tasarım desenleridir. Factory pattern'de bu dörtlüden biridir. Diğerleri; singleton, abstract factory ve repository pattern'dir.
