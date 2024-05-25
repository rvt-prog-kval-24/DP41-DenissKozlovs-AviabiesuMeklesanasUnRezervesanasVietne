# Lietotāja cēļvedis
### Sistēmas prasības aparatūrai un programmatūrai

Sistēma ir izstrādāta tā, lai to varētu izmantot ar daudziem datoru veidiem. Minimālās datora prasības vietnes darbināšanai ir uzskaitītas turpmāk. Šīs prasības ietver gan aparatūras, gan programmatūras komponentus, kas nodrošina stabilu darbību un visu vietnes elementu, tostarp fona video, attēlošanu.


Minimālās prasības

10.Tabula Minimālās prasības

| Nr. | Komponents          | Minimālās prasības                                     |
|-----|---------------------|--------------------------------------------------------|
| 1   | Operētājsistēma     | Windows 7 / MacOS X 10.10 / Linux Kernel 3.10 un jaunāks|
| 2   | Procesors           | Intel Core i3 vai līdzvērtīgs                          |
| 3   | Operatīvā atmiņa     | 4 GB                                                  |
| 4   | Cietais disks       | 2 GB brīvas vietas                                     |
| 5   | Videokarte          | Atbalsts DirectX 11 vai OpenGL 3.3                     |
| 6   | Pārlūkprogramma     | Google Chrome / Mozilla Firefox / Safari (jaunākās versijas) |
| 7   | Interneta pieslēgums | Platjoslas pieslēgums ar ātrumu vismaz 2 Mbit/s       |

Lai palaistu vietni, ir jābūt instalētai pārlūkprogrammai, vietējam XAMPP serverim un interneta savienojumam.
Ir vēlams, lai vietnes darbināšanai būtu šādas lietojumprogrammu versijas: 

* XAMPP 8.0.30 
* XAMPP 8.1.25
* XAMPP 8.2.12

  
### Sistēmas instalācija un palaišana

Sistēmas instalācija un palaišana
Lai uzstādītu un palaistu tīmekļa vietni biļešu pārdošanai, izpildiet šos soļus:

1. Lejupielādējiet vietnes failus

* Lejupielādējiet projekta failus no GitHub krātuves https://github.com/DenKozlov04.
* Lejupielādējiet projekta datu bāzi no Google Drive krātuves https://drive.google.com/file/d/............/view?usp=sharing

2. Uzstādiet XAMPP .

* Instalējiet lokālo serveri XAMPP .
* Uzziniet paroli no administrācijas profila vietnes veidotāja.
3. Konfigurējiet PHP iestatījumus

* Atveriet php.ini failu, kas atrodas XAMPP konfigurācijas mapē.
* Mainiet rindu upload_max_filesize uz 20M, lai atļautu augšupielādēt failus līdz 20 MB.
4. Kopējiet vietnes failus uz serveri

* Kopējiet lejupielādētos vietnes failus uz mapi htdocs, kas atrodas C:\xampp\htdocs.
5. Palaidiet Apache un MySQL serverus

* Atveriet XAMPP vadības paneli un palaidiet Apache un MySQL serverus.
6. Iestatiet datu bāzi

* Atveriet pārlūkprogrammu un ierakstiet adreses joslā http://localhost/phpmyadmin/.
* Izveidojiet jaunu datu bāzi ar nosaukumu airflightsdatabase.
* Izvēlieties tikko izveidoto datu bāzi, spiediet "Importēt" un augšupielādējiet lejupielādēto datu bāzes failu.
7. Palaidiet vietni

* Atveriet pārlūkprogrammu un ierakstiet adreses joslā http://localhost/ jūsu projekta nosaukumu /php/index.php.

Pēc šo soļu izpildes jūsu vietne biļešu pārdošanai būs gatava darbam.

### Programmas aprakasts

1.Autorizācija reģistrētam lietotājam.

Atvetam pārlūkā saiti: http://localhost/main_course_project/php/index.php (skat. ?. att.)
Spiežam uz pogu "Login/Register" vai uz "Search for tickets". Tā kā jus neesat sesijā, tiks atvērta pieteikšanās lapa.

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/mainpage.png)

? att. Index.php jeb sākuma lapas skats  


Ievadam datus un spiežam pogu "LOG IN" (skat. ?. att.)


![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/autorization.png)

? att. Autorizācijas lapas skats

Ja ievaditie dati bija ar lomu "Admin" (skat. ?. att.),tad vērās vaļā administratora panele, bet ja "user", tad parastu lietotāju skats (skat. ?. att.)


![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/adminpage.png)

? att. Administatora lapas skats

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/lietotajalapasskats.png )

? att. Parastā autorizēta lietotāja lapas skats

2.Registrācija jaunam lietotājam.

Uz galvenas lapas spiežam uz pogu "Login/Register"" vai uz "Search for tickets". (skat. ?. att.)
Atvertā autorizācijas lapā, spiežam "Create an account" (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/createaccauntpoga.png )

? att. Registrācijas pogas skats

Ievadam jauna lietotāja datus un spiežam pogu "SING UP" (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/registrpage.png)

? att. Registrācijas lapas skats


3.Komentāru atstāšana.

Kad esat autorizējies tīmekļa vietnē, noklikšķiniet uz pogas "Rewievs" sākumlapā.  (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/revievspoga.png)

? att. Komentāru lapas pogas skats

Uz komentāru lapas, laukā "Add a comment" atstājiet savu komentāru un noklikšķiniet uz pogas "Post".  (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/commentlapa1.png)

? att. Komentāru lapas un komentāru formas skats

4.Komentāru rediģēšana.

Atvēram komentāra lapu? kā autorizēts lietotājs.
Uz komentāru lapas, noklikšķiniet uz pogas "Edit" un rediģējam comentāru (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/komenteditpoga.png)

? att. Komentāru lapas , rediģēšanas logas skats

Noklikšķiniet uz pogas "Edit",kura atrodas rediģēšanas logā (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/redcomment.png)

? att. Komentāru lapas , rediģētas komentāras skats

5.Komentāru dzēšana.

Atvēram komentāra lapu? kā autorizēts lietotājs.
Uz komentāru lapas, noklikšķiniet uz pogas "Delete" (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/deletepoga.png)

? att. Komentāru lapas , dzēšanas pogas skats

6.Biļetes rezervēšana.

Uz galvenas lapas kā autorizēts lietotājs noklikšķiniet uz pogas "Search for tickets".
Lidojumu lapā izvēlieties atbilstošo lidojumu un noklikšķiniet uz "Book a ticket now". (skat. ?. att.) Lidojuma lapā ir arī lauki un poga "Meklēt biļetes", kas pilda tādu pašu funkciju kā sākuma lapa.

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/biletesizveleslapa.png)

? att. Biļetes izvēles lapas skats

Lidojuma informācijas lapā noklikšķiniet uz pogas "Order".

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/infolapa.png)

? att. Lidojuma informācijas lapas skats

Lapā ar pieejamajiem lidojumiem kalendārā izvēlieties piemērotu datumu, pēc tam noklikšķiniet uz lidojuma, kas jums ir piemērots . Lai izdarītu galīgo izvēli, noklikšķiniet uz pogas "Continue".

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/brivaslidojumaizvele.png)

? att. Lapas ar pieejamajiem lidojumiem skats

Izvēlieties sev piemērotāko lidojuma veidu, noklikšķinot uz vienas no biļetēm pogas "Continue".

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/offerlapa.png)

? att. Biļešu klases lapas skats

7.Lidojuma apraksta lapa.


8. Pieejamā lidojuma izvēles lapa.


9. Lidojuma līmeņa izvēles lapa.


10. Klasisko vai biznesa lidojumu izvēles lapa.


11. Aviokompānijas bagāžas atlases lapa.


12. Brīvas sēdvietas izvēlei lidmašīnā lapa.


13. Lietotāja personas datu ievadīšanu pirms maksājuma veikšanas lapa.


14. Administratora mājas lapa.


15. Lidojuma datu modificēšanas lapa.


16.Informācijas lapa par biļešu atcelšanu


17.Informācijas lapa par ceļošanu ar dzīvniekiem


18.Informācijas lapa par bagāžas svaru


19.Informācijas lapa par atlaidēm


20.Informācijas lapa par bagāžas reģistrāciju








