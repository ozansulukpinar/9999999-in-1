## Dictionary

8 Mart 2019

Hashtable: dictionary'nin generic olmayanıdır(non-generic).
Stack & Queue
Stack : Üst üste konan kitaplar olarak düşünebiliriz. Bu sayede ilk başta son konulan kitabı rahatlıkla alabiliriz. Koleksiyonların bu mantıkla çalışan versiyonları diyebiliriz. "ilk giren son çıkar, son giren ilk çıkar"(LIFO:Last in first out).
Pop() : Yığındaki en üstteki elemanı döndürür ve yığından çıkarır
Peek() : Yığındaki en üstteki elemanı döndürür ama yığından çıkarmaz
Push(): İlgili yığının en üstüne o elemanı ekler
Clear() : Tüm elemanları siler.
toArray : Tüm elemanları object dizisi olarak döndürür
Contains() : Olup olmadığını ture/false döner.

Queue : Tam tersidir (FIFO).
Dequeue() : Kuyruğun en başındaki elemanı döndürür ve kuyruktan çıkarır.
Peek() : Kuyruğun en başındaki elemanı döndürür ama yığından çıkarmaz
Enqueue() : Eleman o kuyruğun en sonuna eklenir.
TrimtoSize(): İlgili kuyruğun kapasitesiyle eleman sayısı eşitlenir.
