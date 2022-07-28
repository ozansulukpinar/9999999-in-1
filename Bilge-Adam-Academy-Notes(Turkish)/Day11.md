## Metotlar

27 Şubat 2019

Datetime metotlar
DateTime zaman = new DateTime(2019, 2, 1, 14, 25, 00);
DateTime simdikiZaman = DateTime.Now; //sistem tarihi ve saatini verir.
TimeSpan fark = zaman - simdikiZaman;
DateTime eklenmisZaman = simdikiZaman.Add(TimeSpan.FromDays(20));//şimdiki zamana yirmi gün ekler

            int gunFarki = zaman.Subtract(simdikiZaman).Days;
            DayOfWeek haftaninHangiGunu = DateTime.Now.DayOfWeek;
            DateTime donusturulen = Convert.ToDateTime("27.02.2019");//istem dili formatında yazılmalı
            //datetime içerisindeki spesifik parçaları da yakalayabiliriz.

            int yil = donusturulen.Year;
            int ay = donusturulen.Month;
            int gun = donusturulen.Day;
            int dakika = donusturulen.Minute;

            int buAyKacCekiyor = DateTime.DaysInMonth(DateTime.Now.Year, DateTime.Now.Month);
            DateTime onGunOnce = simdikiZaman.AddDays(-10);

DateTime.IsLeapYear(DateTime.Now.Year)

Math metotlar
int mutlakDeger = Math.Abs(-25);
double asagiYuvarla = Math.Floor(22.56);
int yukariYuvarla = (int)Math.Ceiling(22.56);
int buyukSayi = Math.Max(12, 24);
int kucukSayi = Math.Min(12, 24);
double ussu = Math.Pow(2, 3);
double karekok = Math.Sqrt(16);
double tamSayi = Math.Truncate(2.78); //ondalıklı kısma bakmaz sadce tam kısmını teslim eder
double piSayisi = Math.PI;
double piYuvarlanmis = Math.Round(Math.PI, 2);
int isaret = Math.Sign(-23);
