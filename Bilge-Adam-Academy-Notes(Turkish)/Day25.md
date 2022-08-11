## OOP

19 Mart 2019

### Polimorphism

Çok biçimliliktir.

**Overload:**

- Method overload
- Operator overload
- Override

**Abstract(Soyut) Sınıf:** Abstract class'lar kendisinden kalıtım alacak sınıflara base class olması için yaratılan sınıflardır. Abstract sınıftan instance alınamaz. Abstract sınıf başka bir sınıftan kalıtım alamaz. Abstract sınıflar abstract öğeler içerebilir. Abstract sınıftan kalıtım alan sınıflar base sınıftaki abstract öğeleri implemente etmek zorundadır.

**Sealed Sınıf:** sealed keyword'u sadece sınıflar için değil, override edilmesini istemediğim property ve metotlar için de kullanılabilir. Kesinlikle en üstte olacaksa abstract, kesinlikle en altta/dipte olacaksa sealed keyword kullanılmalıdır. sealed olarak tanımlanan sınıflardan kalıtım alınamaz.

**Interface:** Interface'lerin default access modifier'ı public'tir. Interface'ler kendisini implemente edecek sınıflara çeşitli kabiliyetler kazandırabilmemizi sağlar. Interface tanımlarken onu kullanacak sınıflar için bir şablon oluştururuz. Biz bu şablonla sadece ne yapılacağını belirtiriz. Nasıl yapılacağı sınıfın kendi içerisinde tanımlanır. I ön eki ile başlamalıdır. Interface içinde field tanımlanamaz. Interface'ler başka sınıftan kalıtım alamaz. Ancak içerisine başka bir interface implemente edebilir. Interface içerisinde access modifier kullanılmaz.
