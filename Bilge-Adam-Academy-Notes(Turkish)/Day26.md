## OOP

20 Mart 2019

### IComparable

**Sort():** String sınıfı comparable olduğu için devamlı sıradaki elemanı, compare to metoduna göndererek o anki eleman ile karşılaştırıp, büyüklük küçüklük durumuna göre, koleksiyonu içerisinde sıraya sokmaktadır.

### IDisposable

StreamReader nesnesi yukaridaki scope dışından erişilemez. Çünkü o scope'tan çıktıktan sonra bellekten de düşmüştür. Bunu kalıtım aldığı sınıf olan TextReader sınıfına implemente edilmiş IDisposable interface'i sayesinde yapabilmektedir.
IDisposable olmadığı için ve bu şekilde kullanımda program nesnemizi RAM'den düşürmeye çalışacağından derleme hatası veriyor(çünkü myclassdisposable değil.). Bu noktada nesnemin işi bitip Dispose metodu çalışır.

**Struct:** Değer tipli programlama öğesidir. Struct tanımlamanın class'tan farkı yoktur. Class'lar reference tipli, struct'lar değer tiplidir. Microsoft diyor ki, tip içerisinde taşıyacağınız değer 16 byte'ı geçmiyor ise struct kullanınız, aksi takdirde class kullanınız. Struct'lar kalıtımı desteklemezler ancak kendileri ValueType isimli bir türden kalıtım almışlardır. Struct'lar kalıtım desteklemese de interface implementasyonu yapılabilir. Struct'ların da varsayılan constructor'ı vardır ancak biz onda değişiklik yapamayız sadece parametre alan bir constructor yazabiliriz. Eğer kendimiz bir constructor oluşturuyorsak construction esnasında struct içindeki değerleri initilize etmeliyiz, yani bir değer atamalıyız.

**Enum:** Değer tipli programlama öğeleridir. Programcıya bir listeden elemanlar seçtirmek için kullanılabilir. Her bir elemanın sayısal bir karşılığı vardır. Enum isminde bir class da mevcuttur ve bize enum tipiyle işlem yapabileceğimiz metotlar sunar.
