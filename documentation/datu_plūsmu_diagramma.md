# Datu plūsmu diagrammas 
##Funkcionālais sistēmas modelis
###Datu plūsmu modelis

Datu apstrādes procesi:
*	Paroles maiņa - šīs operācijas laikā (skat. 5. att.) lietotājs nomaina esošo paroli pret jaunu. Lai jaunā parole tiktu saglabāta datubāzē, tai ir sekmīgi jāiztur pašreizējās paroles atbilstības pārbaudes, kā arī aizliegto rakstzīmju un iestatītā garuma atbilstības pārbaudes.

 
6.att. Paroles maiņas  plūsmu diagramma

*	Biļešu rezervāciju pārbaude pirms apmaksas - šīs operācijas laikā (skat. 7. att.) sistēma pārbauda lietotāja sesijas esamību, pasūtījuma esamību un atbilstošo rindu datubāzē. Pēc šīs procedūras notiek pati pasūtījuma apmaksa. 

7.att. Biļešu rezervāciju pārbaude pirms apmaksas plūsmu diagramma

*	Lietotājvārda maiņa - šīs operācijas laikā (skat. 8. att.) lietotājs maina savu esošo lietotājvārdu uz jaunu. Lai saglabātu jauno vārdu, tam ir jāiztur šādas pārbaudes: pārbaude par atļautajām rakstzīmēm, garumu un atbilstību starp pašreizējo vārdu un jauno vārdu.
 
8.att. Lietotājvārda maiņas  plūsmu diagramma

*	Biļešu meklēšana - šīs operācijas laikā (skat. 9. attēlu) tiek apstrādāts lietotāja pieprasījums un lidojumi tiek filtrēti atbilstoši viņa pieprasījumam. Lai filtrēšana varētu notikt, pieprasījumam ir jāiztur šādas pārbaudes: atļautās rakstzīmes, garums. Ja pieprasījums un filtrētie dati sakrīt, šī operācija tiek izpildīta.
 
9.att. Biļešu meklēšanas  plūsmu diagramma

*	Autorizācijas datu apstrāde - šīs operācijas laikā (skat. 10. attēlu) tiek apstrādāti lietotāja autorizācijas dati, ar kuru palīdzību lietotājs piesakās savā esošajā profilā. Lai lietotājs varētu autorizēties, datiem ir jāiztur šādas pārbaudes: derīga garuma, aizliegto rakstzīmju un identitātes pārbaude ar datubāzes datiem. Ja tie nav identiski, autorizācija nenotiek.  
 
10.att. Autorizācijas datu apstrādes  plūsmu diagramma

