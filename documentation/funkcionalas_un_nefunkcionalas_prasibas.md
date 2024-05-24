## Funkcionālās prasības 

1. Jānodrošina iespēja reģistrēt jaunu lietotāju. 
    - Jāparedz ievadīt un pārbaudīt ieejas informāciju par lietotāju. Ja formāts ir nepareizs, vai simbolu skaits ir pārāk liels vai pārāk maz, tad jāizvada paziņojums par nepareizu paroli vai vārdu.
    -	Ja kāds lauks nav ievadīts, tad izvadīt par to kļūdas paziņojumu. 
    -	Salīdzināt ievadīto lietotāja vārdu un citu informāciju ar sistēmā jau eksistējošo lietotāju vārdiem un citai  informācijai, izvadīt paziņojumu, ja tie sakrīt.
      
2. Jānodrošina iespēja autorizet lietotāju.
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam vai jau pastāv datu bāzē, tad tiek izvadīta kļūda.
    -	Ja kāds no laukiem nav ievadīts, izvadīt par to paziņojumu
    -	Ja parole nesakrīt ar atkārtoti ievadīto paroli paroles autorizācijas laukā, tad jāizvada kļūda par nesakritību.
      
3.	Jānodrošina iespēja atstāt komentārus lietotājam.
    -	Ja lietotājs nav iegājis sistēmā, viņš nevarēs atstāt komentārus vietnē.
    -	Ja komentāra garums pārsniedz pieļaujamo parametru, tiks izvadīta kļūda.
      
4.	Jānodrošina iespēja rediģēt komentārus lietotājam.
    -	Lietotājs var rediģēt tikai savus komentārus.
    -	Ja komentāra garums pārsniedz pieļaujamo parametru, tiks izvadīta kļūda.
      
5.	Jānodrošina iespēja dzēst komentārus lietotājam.
    -	Ja lietotājs nav iegājis sistēmā, viņš nevarēs atstāt komentārus vietnē.
    -	Ja komentārs nav pieejams, lietotājs to nevarēs dzēst.
      
6.	Jānodrošina iespēja atstāt komentārus adminam.
    -	Ja admins nav iegājis sistēmā, viņš nevarēs atstāt komentārus vietnē.
    -	Ja komentāra garums pārsniedz pieļaujamo parametru, tiks izvadīta kļūda.
      
7.	Jānodrošina iespēja dzēst visus lietotāja komentārus adminam.
    -	Ja neviens lietotājs nav atstājis komentārus, adminam tiks izvadīta ziņa, ka nav pieejami komentāri.
      
8.	Jānodrošina iespēja dzēst visus lietotāja komentārus adminam.
    -	Ja neviens lietotājs nav atstājis komentārus, adminam tiks izvadīta ziņa, ka nav pieejami komentāri
    -	Ja komentāra garums pārsniedz pieļaujamo parametru, tiks izvadīta kļūda.
      
9.	Jānodrošina iespēja pasūtīt bileti. 
    -	Ja lietotājs nav reģistrējies, tad jāizvada poga ar uzrakstu "Reģistrēties".
    -	Ja lietotājs atkārtoti noklikšķina uz "Pasūtīt biļeti", tiks izvadīta ziņa, ka biļets jau ir pasūtīts.
      
10.	Jānodrošina iespēja pievienot jaunas lidojumus adminam.
    -	Ja kāds no laukiem nav ievadīts, izvadīt par to paziņojumu
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam tad tiek izvadīta kļūda.
      
11.	Jānodrošina iespēja rediģēt jaunas lidojumus adminam.
    -	Ja kāds no laukiem nav ievadīts, izvadīt par to paziņojumu
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam tad tiek izvadīta kļūda.
      
12.	Jānodrošina iespēja dzēst lidojumus adminam.
    -	Ja nav neviena lidojuma, to dzēst nav iespējams.
      
13.	Jānodrošina iespēja rediģēt lidojumus adminam.
    -	Ja rediģēšanas laukumā paliek tukšs vismaz viens lauks, tiks izvadīta kļūda, kas informē par nepieciešamību aizpildīt lauku.
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam tad tiek izvadīta kļūda.
      
14.	Jānodrošina iespēja rediģēt profilu lietotājam.
    -	Ja kāds no laukiem nav ievadīts, izvadīt par to paziņojumu
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam tad tiek izvadīta kļūda.
    -	Salīdzināt ievadīto lietotāja vārdu un citu informāciju ar sistēmā jau eksistējošo lietotāju vārdiem un citai  informācijai, izvadīt paziņojumu, ja tie sakrīt.
    -	Ja profila attēls, kas tika augšupielādēts, ir lielāks par 2 MB, tiks izvadīts paziņojums, ka attēls ir pārāk liels.
      
15.	Jānodrošina iespēja pievienot bērnus lietotājam.
    -	Ja kāds no laukiem nav ievadīts, izvadīt par to paziņojumu
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam tad tiek izvadīta kļūda.
    -	Ja bērna sēdeklītis nav izvēlēts, tiek parādīts paziņojums, ka bērna sēdeklītis ir jāizvēlas.

16.	Jānodrošina iespēja dzēst profilu lietotājam.
    -	Ja tiek nospiesta dzēšanas poga, tiek parādīts operācijas apstiprinājums.
      
17.	Jānodrošina iespēja dzēst bērnus lietotājam.
    -	Ja bērna nav datubāzē, tad būs izvadīta kļūda.
      
## Nefunkcionālās prasības


1.	Dizainam ir jābūt saprotamam un patīkamam lietotājam.
2.	Tekstam jābūt labi redzamam lietotājam un jāizskatās lakoniski kopā ar tīmekļa vietnes noformējumu.
3.	Mājas lapā jābūt instrukcijai par konkrētu darbību veikšanu.
4.	Mājas lapā jābūt iespējai lietotājiem atstāt atsauksmes un komentārus.
5.	Lietotājam profilu jabut saprotamam un ērtam izmantošānā.
6.	Jebkura ievades rinda jāaizsargā pret SQL pieprasījumu ievadi (SQL injekcijām).
7.	Mājaslapai jāstrādā ātri, apstrādājot visu informāciju.
8.	Admina lapai jabut viegli uztvēramai
9.	Adminam jābūt iespējai mainīt visus nepieciešamos datus.
10.	Vajadzības gadījumā lietotājam jābūt iespējai atcelt pakalpojumu.

      
Sistēmas ekrānu skices:
* Galvena lapas skice (skat. 2. att.)

  ![2 att.](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/1.png "2 att.")

1.att. Galvena lapas skices attēls 

* Admina lapas skice.  (skat. 3. att.)

  ![3 att.](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/2.png "3 att.")

2.att. Admina lapas skices attēls

* Lietotāja komentāru sistēmas skice (skat. 4. att.)

  ![4 att.](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/3.png "4 att.")
 
3.att. Komentāru sistēmas skices attēls
