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

Lai palaistu vietni, ir jābūt instalētai pārlūkprogrammai, vietējam XAMPP vai Laragon serverim un interneta savienojumam.
Ir vēlams, lai vietnes darbināšanai būtu šādas lietojumprogrammu versijas: 

* XAMPP 8.0.30 
* XAMPP 8.1.25
* XAMPP 8.2.12
* Laragon v 6.0
* Laragon v 5.0

  
### Sistēmas instalācija un palaišana

Sistēmas instalācija un palaišana
Lai uzstādītu un palaistu tīmekļa vietni biļešu pārdošanai, izpildiet šos soļus:

1. Lejupielādējiet vietnes failus

* Lejupielādējiet projekta failus no GitHub krātuves.
* Lejupielādējiet arī datu bāzes failu.
2. Uzstādiet XAMPP vai Laragon

* Instalējiet lokālo serveri XAMPP vai Laragon.
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
