## XML Serialization

28 Mart 2019

**Serialization(Serileştirme):** .NET üzerinde işlem yaptığımız bir nesnenin, bir sınıfın saklanmak istenilen ya da gönderilmek istenilen formata dönüştürülmesi işlemidir. Böylece nesneyi fiziksel olarak (geçici ya da kalıcı) harddisk'imizde bir dosyaya yazabilir ya da network'e transfer edebilir ya da web servisleri ile gönderebiliriz. Bu işlemler için data'ları seriliaze etmemiz gerekir. Böylece veriler küçülür, daha performanslı hale gelir.

**Deserialization(Ters Serileştirme):** Bir kaynakta bulunan serileştirilmiş belirli bir formdaki nesnelerin, ihtiyaç olduğu çalışma zamanındaki durumunu elde etme işlemidir.
Serileştirme işlemini daha rahat uygulayabilmek için System.Runtime.Serialization namespace kullanılır. Buradan serilizasyon sınıfına erişebilir ve araçları kullanabiliriz, böylelikle nesnelerimizi, datalarımızı istediğimiz formatta saklayabiliriz.
