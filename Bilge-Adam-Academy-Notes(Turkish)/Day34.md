## JSON Binary

1 Nisan 2019

Binary Serilization

Referans tipler, değer tipler, enumerator'ler, delegate'ler için [Serializable] etiketi uygulanabilir. [NonSerialized] serileştirmeye katılmaz, sadece field'lar için kullanılır.

JSON Seriliazition
Memorystream kullanıldığında RAM'e yazıldığı için program kapandığında veri çöp olur.

JSON, XML gibi veri değişim formatıdır. XML'den sonra çıkmıştır, XML'de olduğu gibi hem insanlar tarafından hem de programlama dilleri tarafından okunması ve yazılması kolaydır. JSON programlama dillerinden tamamen bağımsızdır. Ancak C kökenli dillere (C, C++, C#, Java, Javascript, Perl, Python vb..) tanımlama formatı bakımından benzemektedir. Bu özelliğiyle JSON veri değiş tokuş konusunda ideal hale gelmiştir.
JSON temelde Javascript uygulamaları için oluşturulmuş bir veri formatıdır, çıkış amacı ise veri transferlerinde xml'den daha az yer kaplamasını sağlamaktır. Şu an sadece Javascript uygulamalarında değil, yazılım geliştirmede kullanılan birçok teknolojide json
formatında veriler çekilmektedir.
