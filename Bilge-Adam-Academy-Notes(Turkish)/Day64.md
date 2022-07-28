## CSS

15 Mayıs 2019

position: sticky;
z katmanında kendisini kitler, scroll bar'ı hareket ettirdiğimizde olduğu yerde sabit kalır gibi durur. Default position'ı static'tir.
position: fixed;
Logo veya menü için kullanılır, element kadarını sabitler.
position: relative;
Kendi bulunduğu yeri başlangıç noktası olarak baz alıyor.
absolute: Kendi bulunduğu konumdan koparıp dış çerçevenin başlangıç noktasını, başlangıç noktası olarak baz alıyor.

Kombinasyonlar(Combinators)
Büyüktür işareti koyduğumuzda çocuğunu, koymadığımızda(div p) içindeki bütün hepsini seçiyoruz.
child(çocuk) selector
div > p {
font-weight:bold;
}
descendant(torun ya da çocuk) selector
div p{
font-size:25px;
}
adjasent(bitişik) sibling selector, div sonra gelen ilk kardeş
div+p{
color:red;
}
general sibling selector, div sonra gelen bütün kardeşler
div ~ p {
font-style:italic;
}
div elementi olup class'ı ko olanlar
div.ko{
background-color:aquamarine;
}
div'in altında herhangi bir seviyede class'ı list olan ul'ler
div ul.list {
color:purple;
}

PseudoClass
bütün listelerdeki ilk elemanı seçmek istediğimizde
li:first-child{
color:darkorange;
}
bütün listelerdeki son elemanı seçmek istediğimizde
li:last-child{
text-decoration:line-through;
}
1'den başlar, 2. çocuğa git demek için kullanılır
li:nth-child(2){
font-weight:bold;
}
her paragrafın ilk satırına gider
p::first-line{
color:hotpink;
}
her paragrafın içindeki ilk harfi almak için kullanılır
p::first-letter{
font-size:xx-large;
}
h1::before{
content: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRHVRws5KXx9wwHSG70w9IrqCKSAC2P8wgz9rOMltIrPQGEebZR);
}
bir şey taranarak seçildiğinde ne olacağını belirler
::selection{
background-color:red;
color:yellow;
}

            clear:both; etrafındaki şeyleri temizlemeye çalışır
