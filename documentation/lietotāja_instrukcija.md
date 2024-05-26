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

Atvetam pārlūkā saiti: http://localhost/main_course_project/php/index.php (skat. 14. att.)
Spiežam uz pogu "Login/Register" vai uz "Search for tickets". Tā kā jus neesat sesijā, tiks atvērta pieteikšanās lapa.

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/mainpage.png)

14. att. Index.php jeb sākuma lapas skats  


Ievadam datus un spiežam pogu "LOG IN" (skat. 15. att.)


![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/autorization.png)

15. att. Autorizācijas lapas skats

Ja ievaditie dati bija ar lomu "Admin" (skat. 16. att.),tad vērās vaļā administratora panele, bet ja "user", tad parastu lietotāju skats (skat. 17. att.)


![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/adminpage.png)

16. att. Administatora lapas skats

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/lietotajalapasskats.png )

17. att. Parastā autorizēta lietotāja lapas skats

2.Registrācija jaunam lietotājam.

Uz galvenas lapas spiežam uz pogu "Login/Register"" vai uz "Search for tickets". (skat. 14. att.)
Atvertā autorizācijas lapā, spiežam "Create an account" (skat. 18. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/createaccauntpoga.png )

18. att. Registrācijas pogas skats

Ievadam jauna lietotāja datus un spiežam pogu "SING UP" (skat. 19. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/registrpage.png)

19. att. Registrācijas lapas skats


3.Komentāru atstāšana.

Kad esat autorizējies tīmekļa vietnē, noklikšķiniet uz pogas "Rewievs" sākumlapā.  (skat. 20. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/revievspoga.png)

20. att. Komentāru lapas pogas skats

Uz komentāru lapas, laukā "Add a comment" atstājiet savu komentāru un noklikšķiniet uz pogas "Post".  (skat. 21. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/commentlapa1.png)

21. att. Komentāru lapas un komentāru formas skats

4.Komentāru rediģēšana.

Atvēram komentāra lapu? kā autorizēts lietotājs.
Uz komentāru lapas, noklikšķiniet uz pogas "Edit" un rediģējam comentāru (skat. 22. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/komenteditpoga.png)

22. att. Komentāru lapas , rediģēšanas logas skats

Noklikšķiniet uz pogas "Edit",kura atrodas rediģēšanas logā (skat. 23. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/redcomment.png)

23. att. Komentāru lapas , rediģētas komentāras skats

5.Komentāru dzēšana.

Atvēram komentāra lapu? kā autorizēts lietotājs.
Uz komentāru lapas, noklikšķiniet uz pogas "Delete" (skat. 24. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/deletepoga.png)

24. att. Komentāru lapas , dzēšanas pogas skats

6.Biļetes rezervēšana.

Uz galvenas lapas kā autorizēts lietotājs noklikšķiniet uz pogas "Search for tickets".
Lidojumu lapā izvēlieties atbilstošo lidojumu un noklikšķiniet uz "Book a ticket now". (skat. 25. att.) Lidojuma lapā ir arī lauki un poga "Meklēt biļetes", kas pilda tādu pašu funkciju kā sākuma lapa.

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/biletesizveleslapa.png)

25. att. Biļetes izvēles lapas skats

Lidojuma informācijas lapā noklikšķiniet uz pogas "Order".(skat. 26. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/infolapa.png)

26. att. Lidojuma informācijas lapas skats

Lapā ar pieejamajiem lidojumiem kalendārā izvēlieties piemērotu datumu, pēc tam noklikšķiniet uz lidojuma, kas jums ir piemērots . Lai izdarītu galīgo izvēli, noklikšķiniet uz pogas "Continue".(skat. 27. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/brivaslidojumaizvele.png)

27. att. Lapas ar pieejamajiem lidojumiem skats

Izvēlieties sev piemērotāko lidojuma veidu, noklikšķinot uz vienas no biļešu klases pogas "Continue".(skat. 28. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/offerlapa.png)

28. att. Biļešu klases lapas skats

Lapā ar biļešu tipa izvēli izvēlieties "Business" vai "Classic" un noklikšķiniet uz kādas no lapā esošajām radiopoga pogām. Lai apstiprinātu savu izvēli, noklikšķiniet uz pogas "Continue". Lai atgrieztos pie biļešu izvēles, noklikšķiniet uz pogas "Back", kas arī atrodas lapā ar biļetes veida izvēli.(skat. 29. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/tickettypelapa.png)

29. att. Biļešu tipa izvēli izvēlieties lapas skats

Bagāžas izvēles lapā varat izlasīt sīkāku informāciju par pakalpojumiem, noklikšķinot uz "Kas ir rokas bagāža" vai "Kas ir reģistrētā bagāža". Ja vēlaties, varat izvēlēties papildu svaru rokas bagāžai salonā, noklikšķinot uz pogām "+8", "+16", "+24", kas nozīmē attiecīgi 8, 16 un 24 kg.(skat. 30. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/luggagelapa.png)

30. att. Bagāžas izvēles lapās skats

Bagāžas atlases lapā ,"Reģistrētā bagāža" formā, noklikšķiniet uz pogas "+" vai "-", lai atlasītu bagāžas svaru, kas jānogādā tieši lidmašīnas bagāžas nodalījumā. (skat. 31. att.)
Noklikšķiniet uz pogas "Turpināt", lai apstiprinātu savu izvēli.

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/bagazanodalijumsforma.png)

31. att. "Reģistrētā bagāža" formas skats

Lai izvēlētos vietu lidmašīnā, jums ir nepieciešams iepazīties ar informāciju vietu izvēles lapā.(skat. 32. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/lidmasinasvietaslapa.png)

32. att. Lidmašīnas vietas lapas skats

Lai atlasītu atrašanās vietu, noklikšķiniet uz tās. Brīvā vieta ir iekrāsota pelēkā krāsā, aizņemtā vieta ir iekrāsota zilā krāsā, vieta, uz kuras noklikšķinājāt, būs iekrāsota sarkanā krāsā. Zem katras vietas ir norādīta tās cena.(skat. 33. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/vietaskrasas.png)

33. att.  Rezervēšanas sēdvietu pogas skats

Izvēloties sēdvietu, noklikšķiniet uz pogas "Continue", kas atrodas pašā sēdvietu atlases lapas apakšā.(skat. 34. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/continuevietaspoga.png)

34. att.  Izvēlētās vietas apstiprinājuma pogas skats

Lai pabeigtu biļešu rezervāciju, jums jāaizpilda veidlapa, kurā norādīta jūsu personīgā informācija. Kad esat aizpildījis visus datus, noklikšķiniet uz pogas "Send and pay". (skat. 35. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/rezervacijaslapasforma.png)

35. att.  Biļešu rezervāciju lapas skats

Lai pārliecinātos, ka biļete ir veiksmīgi rezervēta, kā autorizēts lietotājs, pārejiet uz savu profilu, nospiežot pogu "Your profile" galvenās lapas vietnes galvenē. (skat. 36. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/profilapoga.png)

36. att.  Profila pogas skats

Lietotāja profila lapā pārbaudiet formu "My reservations". Ja tajā ir ieraksts, tas nozīmē, ka jūsu biļete ir veiksmīgi rezervēta. Jūs varat izdrukāt biļeti, nospiežot pogu "Save as PDF", vai arī atcelt biļeti, nospiežot pogu "Cancel" uz biļetes. (skat. 37. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/manasrezervacijasforma.png)

37. att. "My reservations" formas skats

7.Lietotāja informācijas maiņa.

Lai mainītu informāciju savā profilā, jums jādodas uz lietotāja profila lapu un, noklikšķinot uz pogas ar zīmuļa ikonu, varat mainīt profila attēlu, paroli, tālruņa numuru, e-pasta adresi vai lietotājvardu.Jūs varat arī iziet no sava profila vai atgriezties sākuma lapā, izmantojot pogas "Back" un "Logout". (skat. 39. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/mansprofils.png)

38. att. "My profile" formas skats

8. Dažādu funkciju izmantošana.
   
Formā ar dažādu informāciju jūs varat izdzēst profilu, nospiežot pogu "Click here". Privātuma politiku var izlasīt, nospiežot pogu "Privacy policy". Jūs varat pievienot bērnu, aizpildot formu un nospiežot "Add child", ja jums ir reiss. Nospiežot pogu "Choose seat", jūs izvēlēsieties vietu bērnam. (skat. 39. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/dazadasfunkcijas.png)

39. att. "Various functions" formas skats

9. Lidojuma pievienošana .

Lai pievienotu jaunu lidojumu, autorizējieties kā administrators un aizpildiet lidojuma pievienošanas formu. Noklikšķiniet uz pogas "Choose File", lai pievienotu lidojumu, un pēc tam noklikšķiniet uz pogas "Add flight". (skat. 40. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/adminforma.png)

40. att. Admina formas skats

10. Lidojuma rediģēšana.
    
Lai rediģētu vai dzēstu lidojumu, dodieties uz lidojumu lapu kā administrators un noklikšķiniet uz "Dzēst", lai to dzēstu, vai uz zīmuļa ikonu, lai rediģētu. (skat. 41. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/edit.png)

41. att. Lidojuma rediģēšanas skats

Kad noklikšķināsiet uz "rediģēt", tiks atvērta forma datu maiņai, kurā jūs varat rediģēt lidojumu. (skat. 42. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/editforma.png)

42. att. Lidojuma rediģēšanas formas skats

10. Konkrētā datumā pieejamo reisu pievienošana.

Lai pievienotu pieejamu reisu konkrētajai datumei, jums jāieiet "lidojumā", lapā ar kalendāru, kā administrators. Uz lapas parādīsies forma reisa pievienošanai. Aizpildot to, jūs pievienosiet reisu konkrētam lidojumam. (skat. 43. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/addreissforma.png)

43. att. Konkrētā datumā pieejamo reisu formas skats


### Testa piemērs

Kā piemēru testam apskatīsim reģistrāciju, autorizāciju un komentāra atstāšanu. Atverot saiti http://nosaukums_mapē_ar_vietni/php/index.php, mēs redzam galveno lapu. Nospiežot pogu "Your Profile" vai "Search for tickets". (skat. 44. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/mainlapa.png)


Mums atvērsies autorizācijas forma, kurā, aizpildot visus laukus, jūs varēsiet autorizēties. Pēc tam nospiediet pogu "LOG IN", lai nosūtītu formu.(skat. 45. att.)

![](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/autor.png)

