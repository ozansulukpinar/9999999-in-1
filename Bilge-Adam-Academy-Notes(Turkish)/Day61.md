## Entity Framework Code First

10 Mayıs 2019

DbContext
TPC(Table per Concrete)
TPT(Table per Type)
TPH(Table per Hierarchy)

TPC: Concrete class'lar(öğrenci-öğretmen) için ayrı ayrı tablolar oluşur, kalıtımdan gelenleri her tabloya ekler.
TPH: Bir tane kişi tablosu var(base class) bütün class'lardaki property'ler kişi tablosunda toplanır, ekstra bir kolon eklenir, bu kolon discriminator olarak isimlendirilir, bu kolona hangi class'tan instance alındıysa o yazılır, diğer instance alınmayan class'ları null geçer.
TPT: Her tip için tablo yaratır, hiyerarşik olarak kalıtım veren tablo(base class) ile kalıtım alan tablolar(child class) arasında birebir ilişki kurulur.
