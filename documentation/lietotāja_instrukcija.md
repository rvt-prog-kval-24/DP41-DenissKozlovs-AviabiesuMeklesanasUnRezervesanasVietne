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
Spiežam uz pogu "Autorizēties/reģistrēties" vai uz "Meklēt biļetes". Tā kā jus neesat sesijā, tiks atvērta pieteikšanās lapa.

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/mainpage.png)

? att. Index.php jeb sākuma lapas skats  


Ievadam datus un spiežam pogu "LOG IN" (skat. ?. att.)


![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/autorization.png)

? att. Autorizācijas lapas skats

Ja ievaditie dati bija ar lomu "Admin" (skat. ?. att.),tad vērās vaļā administratora panele, bet ja "user", tad parastu lietotāju skats (skat. ?. att.)


![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/mainpage.png)

? att. Administatora lapas skats

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/Datubāzes_fiziskās_struktūras_shēma.png )

? att. Parastā autorizēta lietotāja lapas skats

2.Registrācija jaunam lietotājam.

Uz galvenas lapas spiežam uz pogu "Autorizēties/reģistrēties" vai uz "Meklēt biļetes". (skat. ?. att.)
Atvertā autorizācijas lapā, spiežam "Create an account" 

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/Datubāzes_fiziskās_struktūras_shēma.png )

? att. Registrācijas pogas skats

Ievadam jauna lietotāja datus un spiežam pogu "SING UP" (skat. ?. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/Datubāzes_fiziskās_struktūras_shēma.png )

? att. Registrācijas lapas skats


3.Autorizācijas lapa.


4.Komentāru lapa.


5.Lietotāja profila lapa.


6.Filtrētas biļetes lapa.


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








