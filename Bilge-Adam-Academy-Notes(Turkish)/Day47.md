## ADO.NET

18 Nisan 2019

Connection Strings
ADO.NET(ActiveX Data Objects.NET): ActiveX tabanlı çalışan, Microsoft'un veri erişim teknolojisidir. Veritabanındaki bilgileri elde etme veya veritabanında bulunan verileri değiştirmek için geliştirilmiş bir veri erişim aracıdır. ADO.NET, .NET sınıf kütüphanesindeki System.Data isim alanındaki sınıfların tamamını temsil eder. Bu veri erişim, sadece SQL değil, Oracle, MySQL, Access/OleDB, ODBC gibi tüm database'lere erişim imkanı sunmaktadır. Veri okuyabilir, veri ekletebilir, veri güncelleyebilir ve veri silebiliriz.
ADO.NET'in veri tabanına iki tür bağlantı şekli vardır;

- Connected
- Disconnected

DataAdapter: Gönderdiğimiz sorgu sonucu gelen veriyi geçici hafızaya alan sınıfımızdır(SQLDataAdapter, OleDbDataAdapter, OracleDataAdapter). DataAdapter ile database'den veriyi çekeriz, fakat alınan veriyi kullanabilmemiz için DataTable ve DataSet gibi veri türüne dönüştürmemiz gerekir. Disconnected bağlantılar için kullanılır.

SQL Bağlantısı birinci yöntemi
//windows authentication ile bağlandık.

Server(data source):Bağlanacağınız bilgisayarın adı ya da IP numarası belirtiriz. Localhost kullanıldığında ismi localhost ya da "."(nokta) yazarak belirtilebilir.
Database: bağlanacağınız database'in adını birebir aynı!
User ID(uid/UID): Bağlacağınız veritabanına hangi kullanıcı adı ile gireceğimizi belirtiriz.
Password(pwd/PWD): User ID'mizin şifresini belirtiriz.

Server(data source):Bağlanacağınız bilgisayarın adı ya da IP numarası belirtiriz. Localhost kullanıldığında ismi localhost ya da "."(nokta) yazarak belirtilebilir.
Database: Bağlanacağınız database'in adını birebir aynı!
User ID(uid/UID): Bağlacağınız veritabanına hangi kullanıcı adı ile gireceğimizi belirtiriz.
Password(pwd/PWD): User ID'mizin şifresini belirtiriz.

        //SQL bağlantısı ikinci yöntem-Globalde tanımlama
        /*Global scope'ta SQl nesnesi oluşturulur(constructor metodunun hemen altına)
         */

        //SQL bağlantısı üçüncü yöntem-class ile tanımlama
        //Tools isminde oluşturduğumuz class içinde ConnectionString tanımladık ve Form'da çağırdık.

        //sql bağlantısı dördüncü yöntem-app.config ile tanımlama
        //App.config veya Web.config içinde oluşturduğumuz bağlantıyı burada çağırdık.
        SqlConnection cnnAppConfig = new SqlConnection(ConfigurationManager.ConnectionStrings["baglanti"].ConnectionString);

            //ConfigurationManager:references sağ tık > add reference > System.Configuration eklenmesi gerekir.
