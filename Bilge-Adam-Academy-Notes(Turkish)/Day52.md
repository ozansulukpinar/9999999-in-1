## N-Tier Introduction

26 Nisan 2019

**Modüler Programlama:** Kod yönetilebilirliği, anlaşılabilirlik, projeyi daha sonradan geliştirebilmek, hata olduğunda nereye bakacağını daha kolay anlamak için modüler programlama yapmak gerekir.

Modülerlik metottan başlar, sonrasında class sonra proje olarak genişletilebilir.

**DAL(Data Access Layer,Veri Katmanı):** Veriye erişim katmanıdır, veri çekmek ve göndermekten başka sorumluluğum yoktur.

### Business Logic Layer - İş Mantığı Katmanı

**BLL(Business Logic Layer)(iş katmanı):** İş katmanı varolan iş kurallarının kodlandığı bölümdür. Mesela bir validation(veri tabanına gidecek verinin uyması gereken kurallar) olsun; Northwind'de kategori boş geçilemez ve 15 karakterden fazla olamaz, olursa hata verir, bu bir iş kuralı. Ya da sepette 100 lira ve üstü alışveriş yapıldığında %10 indirim var, bunu yapmak ve yönetmek BLL'in işidir.

**UI)User Interface( Kullanıcı Katmanı):** Tek işi kullanıcıya veri göstermek ve kullanıcıdan veri almak. Bir kontrol yapamaz. UI birden fazla olabilir. UI yerine PL(Presentation Layer) de denir. UI kesinlikle DAL'ı bilmez. UI BLL'i tanır, BLL DAL'ı tanır.

**Entity:** Entity veritabanındaki tabloların class karşılığıdır. Her entity bir classtır, her class bir entity değildir. Entity katmanı her katmanda ekli olması gerekir yani tanıştırılması gerekir.
