## Design Pattern

31 Mayıs 2019

### Repositories Pattern(Kurumsal Pattern)

Kurumsal pattern olduğu için kurumsal mimaride kullanılır, framework oluşturmak için kullanılır. BLL DAL'ı kullanırken daha bağımsız bir yapı kurmak için kullanılır. Katmanlı mimaride getirdiği ya da getirebileceği sıkıntıları çözmek için ortaya çıkmıştır. Veriye erişimin yoğun olduğu uygulamalarda kullanılabilecek bir pattern'dir. CRUD işlemlerini kolaylaştırmış oluruz.

**Not:** Repositories Pattern framework yazarken kullanılır, öylesine kullanılmaz.

Örneğin, projeyi geliştirirken sadece UI ya da sadece veri kısmı değişecekse standart bir şablona ihtiyaç duyulur, kalan kısımlar aynı olsun ama değişecek kısımlar güncellensin dendiğinde Repositories Pattern kullanılır.

### Generic Repositories

Aynısının generic versiyonudur.
Örneğin, kodu bir kere yaz, bütün CRUD işlemleri yapılsın.
Core katmanı işin çekirdek kısmıdır, core katmanını alıp başka bir projeye koyarsak orada da çalışır. Çünkü bu Generic Repositories'dir.
DAL katmanındaki CRUD işlemlerinin belli bir standartta olacağını core katmanı belirler.
Örneğin, Entity'ler de bir class'tır ama diğer class'lardan ayrılması için bir kural koyacaksak bunu core katmanında yaparız.
