## ASP.NET

27 Mayıs 2019

Trace
Page life cycle'daki süreleri ve ayrıntıları görmek için Trace seçeneği true yapılır.
Butona basıldığında asp:TextBox'taki verinin kaybolmaması state management' tır.
State Management: Durum Yönetimi
HTTP protokolü stateless(durumsuz) bir protokoldür.
Sayfanın önceki durumunu bilmez.
HTTP protokolü => Carpe diem! - o an için veriyi tutuyor.
HTTP'nin bu stateless durumunu ortadan kaldırmak için state management ortaya çıkmıştır.
Tüm programlama dillerinde state management mekanizması vardır.

            ASP.NET'te beş tane state management vardır, iki kısma ayrılır:
            1) Server Side
                a) Session
                b) Application (uygulama bazlı)
            2) Client Side
                a) Query String (bir şeyleri linke yönlendirerek)
                b) View State (uygulama esnasındaki verilerin tutulması)
                c) Cookie (çerezler)

QueryString

ViewState
ViewState CSS'leri de tutar.
ViewState default'ta her zaman vardır ve default değeri true'dur.
EnableViewState= false olduğunda tarayıcıda sayfa kaynağını görüntüle dediğimizde ViewState'lerde herhangi bir şey tutulmadığını görürüz, default olan yani true bıraktığımızda tüm veriler ViewState'te şifrelenmiş olarak tutulur.

Cookie: İnternet sitelerinin bilgisayarımıza kaydettiği küçük metin dosyalarıdır. Kullanım amacı, kullanıcı kimlik doğrulama ve tanımlama, kullanıcı tercihleri, alışveriş sepeti vs. bilgileri client tarafında tutmak için.

Session: Oturum bazlı çalışır, her kullanıcı için ayrı bir bağlantı oluşturulur ve o bağlantı içine istediğin gibi veri atıp tutabilirsin. Session cookie ile çalışır, sebebi her oturumda farklı session ID vardır ve bunlar kullanıcılara cookie olarak tanımlanmalıdır, çünkü bu ID'lerden yakalayıp bulur. Session default 20 dakika süresi vardır.

Bu metot herhangi bir session başlatıldığında çalışır.
Application.Lock(); Her oturum açıldığında uygulamayı kitliyoruz, kitlendikten sonra sayıyoruz.
lock durdurur, çünkü aynı anda iki kişi uygulamaya girdiğinde ikisini bir kişi sanmasın diye arada durdurur(kilitler).
Application.UnLock(); Kilidi açar

Güvenli çıkış olayı yazılmazsa tarayıcı kapanır kapanmaz session düşmeyeceği için tarayıcıda direkt göremeyiz, 20 dakika beklemek gerekir.
Güvenli çıkış olayını yazmak gerekli ve önemli, çünkü session kapanınca askıda kalma süresi (20 dakika) var.
Kullanıcılardan biri tarayıcı kapatınca(session düşünce) kişiyi azaltır.
