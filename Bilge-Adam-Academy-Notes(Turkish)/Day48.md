## ADO.NET

19 Nisan 2019

//ExecuteReader: Bu metot genelde SQL cümleciği select komutu içerdiği durumlarda kullanılır, select komutu ile veritabanından bir sorgu yapılarak kayıt kümesi elde edilir, bu kayıt kümesi SqlDataReader nesnesine aktarılır. SqlDataReader ile bu kayıt kümesinden çeşitli yollardan veriler elde edilir.

        //SqlDataReader: Bu nesne ile bir kayıttan sadece ileriye doğru ilerleme yapılır, yeni bir kayıt kümesinden bir kayıt okuduktan sonra tekrar geriye dönüp eski kayıtları okumak mümkün değildir.
        //SqlDataReader açık bir bağlantı ister.

        //Not: ExecuteReader geriye SqlDataReader döndürür, SqlDataReader'ın Read metodu her çalıştığında veri olup olmadığını true-false olarak döndürür.

        /*ExecuteNonQuery:
         * Bu metodu genellikle bir veritabanındaki kayıtları değiştirmek, silmek ya da kayıt eklemek istediğimizde kullanırız. Bu metodun geri dönüş değeri komutun çalıştırıldıktan sonra etkilediği kayıt sayısıdır.
         */
