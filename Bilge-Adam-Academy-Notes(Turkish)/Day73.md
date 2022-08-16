## SOLID

28 Mayıs 2019

OOP'un ucunu kaçırmamak için kurallar vardır. Bunlar:

- Temiz kod
- Kendini tekrar etme
- İhtiyacın olmayan şeyi yapma
- Yazılan kodlar tekrar kullanılabilir olmalı
- Okunabilirliği yüksek
- Geliştirmeye açık

Yukarıda bahsettiklerimiz zamanla prensipleşmiş ve beş temel prensip olmuştur. Kalıplaşmış olanlar:

- Single Responsibility Principle ~ Tek Sorumluluk İlkesi
- Open Close Principle ~ Açıp Kapama İlkesi
- Liskov's Substitutıon Principle ~ Liskov's Yerdeğiştirme İlkesi
- Interface Segregation Principle ~ Arayüz Ayırma İlkesi
- Dependency Inversion Principle ~ Bağımlılığı Ters çevirme İlkesi

Kalıplaşmamış ama yine de OOP prensibi olan; YAGNI(You Ain't Gonna Need It), KISS(Keep It Simple-Stupid), DRY(Don't Repeat Yourself) ...

### Single Responsibility Principle - Tek Sorumluluk İlkesi

Her iş ya da her sorumluluk tek bir şeye ait olmalı(İsviçre çakısı olma-kullanma!).
Örneğin, bir class var ve üzerinde değişiklik yapıldığında hem DAl hem de UI katmanı etkileniyorsa burada bu prensibe uyulmamış demektir!
Eğer bir iş birden fazla işe bölünebiliyorsa bölünmelidir. Bu bize modülerliği sağlar.

### Open Close Principle - Açıp Kapama İlkesi

Değişime kapalı, gelişime açık olmaktır.
Bir projeye, bir yazılıma, bir uygulamaya yeni bir istek gelmiyorsa, geliştirilmiyorsa piyasada ömrü bitmiş demektir.
Bir projeye yeni bir istek geldiğinde var olan kodlarını değiştirmeden yeni kodlar yazarak geliştiriliyorsa bu prensibe uyar.

### Liskov's Substitution - Liskov'un Yerdeğiştirme İlkesi

Liskov der ki; üst tipler(base'ler) hiyerarşide aşağıdaki tiplerin(alt tiplerin) yerine geçebilmelidir.
Bir abstract class'tan implement alınırken implement ettiğin tüm metotların içini doldurman gerekir. Eğer base'den implement edip yani metot getirip içi doldurulmazsa bu prensibe uyulmamış olur.

### Interface Segregation Principle - Interface'leri Ayır Prensibi(Arayüz Ayırma İlkesi)

Bir önceki prensipte bahsettiğimiz durumu uygulamak için metotlara göre, kullanılacak durumlara göre interface'leri ayırırız.

### Dependency Inversion Principle - Bağımlılığı Tersine Çevirme İlkesi

Üst seviye işlemler alt seviye işlemlere bağımlı olmamalı, tam tersi olmalı!

- Alt seviye işlem: Loglama
- Üst seviye işlem: Entity class'ının içinde yapılan işlemler

Örneğin, Entity içinde loglama ile ilgili işlem yazılırsa bu prensibe aykırı olur, bunun yerine loglama işini interface yapıp bu interface üzerinden başka bir class'ta işleri yapmak daha doğru olur.
