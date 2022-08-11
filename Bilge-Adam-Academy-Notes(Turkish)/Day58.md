## Entity Framework

7 Mayıs 2019

**ORM(Object Relation Mapping):** İlişkisel veritabanı(rdbms) ile nesneye yönelik programlamanın(OO) arasında bir köprü özelliği gören ve ilişkisel veritabanındaki bilgilerimizi yönetmek için, nesne modellerimizi kullandığımız bir tekniktir/metottur/programlama teknolojisidir.

## Entity Framework:##

- **Database First (DbFirst)**: Eğer bir veritabanı varsa bu yaklaşım tercih edilir, bu yöntemde veritabanı üzerinde bir değişiklik yapmak istenirse değişiklik SQL tarafında yapılır ve değişikliğin projeye yansıması için "update model form database" tıklanması gerekir.
- **Model First:** Eğer bir veritabanı yoksa ve direkt Visual Studio üzerinden model kullanarak oluşturmak isterseniz tercih edilebilir, veritabanının SQL'e yansıması için "generate database from" tıklanır. Kod yazmayı sevmiyorsanız tercih edilebilir ama en az (neredeyse hiç) kullanılan yaklaşımdır.

**Code First:** Kod yazmayı çok seviyorsanız veritabanını kodla oluşturmak için kullanılır. Veritabanı genelde yoktur ve kodlarla C# tarafında oluşturulur. Veritabanı varsa da code first kullanılabilir. Tablo sayısı az olan projelerde tercih edilir.
