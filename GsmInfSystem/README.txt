Arda Kaşıkçı 18011092

-Information System for Service Providers-

**ÖNEMLİ: Programda yapılan işlemlerin kaydedilmesi için ana pencere kapatılırken SAVE&EXİT butonu kullanılmalıdır. Aksi halde yapılan işlemler kayıt olmayacaktır.

Uygulamada file operations save işlemleri için ve java gui arayüz için kullanılmışır
Bunlar için ekstra olarak 
-AddService
-Database
-FindServ
classları tanımlanmıştır. File operationslarda Service Providerları kaydedip program
tekrar çalıştığında kaydedilmiş bilgilerin sürekliliğini sağladım.
Program InformationSystem classının çalıştırılmasıyla çalışmaya başlar.
Önünüzde 5 seçenek bulunur.

-Add Service Provider
Sisteme yeni Service Provider eklenmesini sağlar.Tıkladığınızda öncelikle size GSM mi Cable mı diye sorar. Burada seçim yaptıktan sonra Service Provider bilgilerini sizden almaya başlar.Sistemde önceden kayıtlı service provider isimleriyle eşleşen bir isim girildiğinde hata alırsınız.Her Service Provider için en az 1 subscription plan tanımlamalısınız.Aksi halde program hata vericektir.

-Add Possible Customer
Öncelikle herhangi bir customer eklemek için önceden Service Provider eklemek zorunludur, aksi halde program hata vericek şekilde kodlanmıştır.
Sistemde iki tip customer vardır biri existing biri possibledır. Possible customer eklerken bu customerın hangi service providerın olası müşterisi olduğunu bilmemiz için başta var olan service providerlardan birinin ismi alınır. Sonrasında ise müşteri bilgileri alınır.

-Add Subscription
Existing customerla beraber subscription tanımlamak için yapılan bir butondur.
Öncelikle herhangi bir customer eklemek için önceden Service Provider eklemek zorunludur, aksi halde program hata vericek şekilde kodlanmıştır.
Öncelikle subscription bilgisi için service provider ismi alınır. Sonrasında kişi biliglerinin hepsi alınıcak şekilde kodlanmıştır. Kişi bilgileri alındıktan sonra subscription tarihi(dd/MM/yyyy şeklinde girilmelidir) ve susbcription plan ismi(Service Providerın var olan bir planı girilmelidir.) alınır. Ardından subscription ve Existing Customer tanımlanır.

-Find Service Provider and Get Inf
Burada sizden var olan service providerın ismi alınır ve service provider bilgileri listelenir. Customerlar ve Subscription Plans listelenir.

-Find Customer and Get Inf
Burada sizden var olan bir customerın citizenship numberı alınır. Ve veritabanında o numaralı customer aranır.Ardından customer bulunursa, Possible customer için ayrı, Existing customer için ayrı bilgiler gösterilir.

Not: Unit Test classı eklenmiştir.
Not: Proje dosyasında olan:Your program shall keep track of records of Existing Customers as well as records of Possible Customers who may have shown interests. 
İfadesi için possible customerları service providerlar içinde tuttum. Çünkü hangi service providerın olası müşterisi bilgisinin bizim için önemli olacağını düşündüm.
Not:MSA array list kullanımına izin verdiği için array list kullandım.