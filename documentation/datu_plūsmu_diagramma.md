# Datu plūsmu diagrammas 
## Funkcionālais sistēmas modelis
### Datu plūsmu modelis

Datu apstrādes procesi:
*	Paroles maiņa - šīs operācijas laikā (skat. 6. att.) lietotājs nomaina esošo paroli pret jaunu. Sākotnēji tiek pārbaudīts, vai sesija ir derīga, un tiek iegūts lietotāja sesijas identifikators. Lai jaunā parole tiktu saglabāta datubāzē, tai ir sekmīgi jāiztur pašreizējās paroles atbilstības pārbaudes, kā arī aizliegto rakstzīmju un iestatītā garuma atbilstības pārbaudes. 

![DP41 Deniss Kozlovs Datu plūsmu diagramma 1](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/plusmudiagr1.png "DP41 Deniss Kozlovs Paroles maiņas  plūsmu diagramm")

6.att. Paroles maiņas  plūsmu diagramma

*	Biļešu rezervāciju pārbaude pirms apmaksas - šīs operācijas laikā (skat. 7. att.) sistēma pārbauda lietotāja sesijas esamību, pasūtījuma esamību un atbilstošo rindu datubāzē. Pēc šīs procedūras notiek pati pasūtījuma apmaksa. 

![DP41 Deniss Kozlovs Datu plūsmu diagramma 2](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/plusmuDiag2.png "DP41 Deniss Kozlovs Biļešu rezervāciju pārbaude pirms apmaksas plūsmu diagramma")

7.att. Biļešu rezervāciju pārbaude pirms apmaksas plūsmu diagramma

*	Lietotājvārda maiņa - šīs operācijas laikā (skat. 8. att.) lietotājs maina savu esošo lietotājvārdu uz jaunu. Lai saglabātu jauno vārdu, tam ir jāiztur šādas pārbaudes: pārbaude par atļautajām rakstzīmēm, garumu un atbilstību starp pašreizējo vārdu un jauno vārdu. Sākotnēji tiek pārbaudīts, vai sesija ir derīga, un tiek iegūts lietotāja sesijas identifikators.

![DP41 Deniss Kozlovs Datu plūsmu diagramma 3](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/plusmuDiag3.png "DP41 Deniss Kozlovs  Lietotājvārda maiņas  plūsmu diagramma") 

8.att. Lietotājvārda maiņas  plūsmu diagramma

*	Biļešu meklēšana - šīs operācijas laikā (skat. 9. attēlu)sistēma pārbauda lietotāja sesijas esamību, tiek apstrādāts lietotāja pieprasījums un lidojumi tiek filtrēti atbilstoši viņa pieprasījumam. Lai filtrēšana varētu notikt, pieprasījumam ir jāiztur šādas pārbaudes: atļautās rakstzīmes, garums. Ja pieprasījums un filtrētie dati sakrīt, šī operācija tiek izpildīta. 

![DP41 Deniss Kozlovs Datu plūsmu diagramma 4](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/plusmuDiag4.png "DP41 Deniss Kozlovs Biļešu meklēšanas  plūsmu diagramma") 

9.att. Biļešu meklēšanas  plūsmu diagramma

*	Autorizācijas datu apstrāde - šīs operācijas laikā (skat. 10. attēlu) sistēma pārbauda lietotāja sesijas esamību, tiek apstrādāti lietotāja autorizācijas dati, ar kuru palīdzību lietotājs piesakās savā esošajā profilā. Lai lietotājs varētu autorizēties, datiem ir jāiztur šādas pārbaudes: derīga garuma, aizliegto rakstzīmju un identitātes pārbaude ar datubāzes datiem. Ja tie nav identiski, autorizācija nenotiek. 

![DP41 Deniss Kozlovs Datu plūsmu diagramma 5](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/plusmuDiag5.png "DP41 Deniss Kozlovs Autorizācijas datu apstrādes  plūsmu diagramma") 

10.att. Autorizācijas datu apstrādes  plūsmu diagramma

*	Talruņa maiņa - šīs operācijas laikā (skat. 11. attēlu) sistēma pārbauda lietotāja sesijas esamību, lietotājs nomaina esošo talruņa numuru pret jaunu. Lai jaunā talruņa tiktu saglabāta datubāzē, tai ir sekmīgi jāiztur pašreizējās talruņa atbilstības pārbaudes, kā arī aizliegto rakstzīmju un iestatītā garuma atbilstības pārbaudes ka arī numuram jāiztur datubāzes atbilstības pārbaude .

![DP41 Deniss Kozlovs Datu plūsmu diagramma 6](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/plusmuDiag6.png "DP41 Deniss Kozlovs Autorizācijas datu apstrādes  plūsmu diagramma") 

11.att. Talruņa maiņas plūsmu diagramma

*	Vietas izvēle - šīs operācijas laikā (skat. 12. attēlu) sistēma pārbauda lietotāja sesijas esamību, tiek apstrādāti lietotājam izvelēta vieta un vietas cēna.Ja kāda iemesla dēļ lietotāja vieta nav izvēlēta vai ir kādas kļūdas, biļešu un kuponu dati netiks pārsūtīti uz datubāzi.  Ja viss notiks bez problēmām, dati tiks pārnesti uz datubāzi. 

![DP41 Deniss Kozlovs Datu plūsmu diagramma 7](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/plusmuDiag7.png "DP41 Deniss Kozlovs Autorizācijas datu apstrādes  plūsmu diagramma") 

12.att. Sēdvietas izvēles plūsmu diagramma
