## Generics

2 Nisan 2019

Generic Types
Farklı veri kaynaklarından veri çekerken çekme işleminin sonucunun her ne tip olursa olsun karşılanabilmesi için generic class yazılır. Nasıl metotlara parametre gönderiyorsak tipi de parametre yapmak istediğimizde generic yapmamız gerekir.

GenericConstraints
{
interface ISample<T>

      where T : class   //=> reference type constraint
      where K:struct    //=> value type constraint
                        //where T:ICollection //type constraint
                        //where T:ICollection,IEnumerable
                        //where T:ICollection,IDisposable
                        //where T: new() //constructer constraint: bunu implement edecek tipler muhakkak default yani parametresiz ctor'a sahip olmak zorunda
                        //where T: class,new() //birden fazla new() için yazılır, her zaman en sonda olacak
