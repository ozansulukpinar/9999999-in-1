## ADO.NET

22 Nisan 2019

SQL Injection: Ekrandan değer alınan alanlar, string birleştirme ile sorguya eklenmez!SQL INJECTION! Bu şekilde kod olmaz, olmaması gerekir.  
Parameters olarak gönderilen değerler, ilgili kolon veri olarak girilmeye çalışır, SQL Injection'ı önler. SQL Injection veritabanından ve dilden bağımsız olarak her türlü uygulama-veritabanı ilişkisine sahip sistemde bulunabilir ve bu veritabanlarının bir açığı değildir, SQL Injection'dan korunmak web geliştiricisinin görevidir.

//CommandBehavior: SqlDataReader nesnesi işlemi bittikten sonra otomatik olarak kapatılır.
