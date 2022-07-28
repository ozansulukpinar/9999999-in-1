## JavaScript

17 Mayıs 2019

setInterval(): İçine aldığı kod bloğunu belli bir saniyede çalıştırır, ikinci parametre olarak saniye cinsinden süre verilir.

DOM: Document Object Model
HTML ile programlama dilleri arasında bir standart oluşturulur ve bu dillerin HTML'den bilgi alıp vermesine yardımcı olur.
DOM'da HTML ile hazırladığınız sayfa ya da belge içindeki tüm öğeler nesne olarak isimlendirlir.
Javascript ile bu öğeleri dinamikleştiririz.

>

Selectors
document.getElementById('pId');
id niteliği ile eşleşen ilk kaydı getirir

        document.getElementsByName('pName');
        name niteliği ile eşleşen tüm kayıtları dizi olarak getirir.

        document.getElementsByClassName('pClass');
        class niteliği ile eşleşen tüm kayıtları dizi olarak getirir.

        document.getElementsByTagName('p');
        etiket adı ile eşleşen tüm kayıtları dizi olarak getirir.

        document.querySelector('p');
        seçici ile eşleşen ilk kaydı getirir.

        document.querySelectorAll('p');
        seçici ile eşleşen tüm kayıtları dizi olarak getirir.

        document.anchors:sayfadaki tüm bağlantılara ulaşmak için
        document.body:body nesnesine ulaşır
        document.documentElement:HTML kökünden itibaren dökümana ulaşmak için

        body,head,documentElement,title tek bir nesne döndürür, diğerleri nesnelerden oluşan dizi döndürür.
        innerHTML: Etiketin içini okuma ve değiştirme için kullanılır, HTML etiketleri de eklenebilir.
        innerText: Etiketin içini okuma ve değiştirme için kullanılır.

        setAttribute(): Etiketin niteliğini değiştirmek için kullanılır.
        style.property: Etiketin stilini değiştirmek için kullanılır.

        classList: Etiketlerin class niteliği üzerinde silme, değiştirme, ekleme, class listesi öğrenme gibi işlemler

        HTML etiketi ekleme ve silme
        document.createElement(element): HTML etiketi oluşturur.
        document.removeChild(element): HTML etiketi siler.
        document.appendChild(element): HTML etiketi ekler.
        document.replaceChild(element): HTML etiketini değiştirir.
