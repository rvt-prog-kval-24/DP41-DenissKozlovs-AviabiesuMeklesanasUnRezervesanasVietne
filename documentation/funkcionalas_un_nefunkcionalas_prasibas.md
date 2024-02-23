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
      
6.	Jānodrošina iespēja atstāt komentārus darbiniekam.
    -	Ja darbinieks nav iegājis sistēmā, viņš nevarēs atstāt komentārus vietnē.
    -	Ja komentāra garums pārsniedz pieļaujamo parametru, tiks izvadīta kļūda.
      
7.	Jānodrošina iespēja dzēst visus lietotāja komentārus darbiniekam.
    -	Ja neviens lietotājs nav atstājis komentārus, darbiniekam tiks izvadīta ziņa, ka nav pieejami komentāri.
      
8.	Jānodrošina iespēja dzēst visus lietotāja komentārus darbiniekam.
    -	Ja neviens lietotājs nav atstājis komentārus, darbiniekam tiks izvadīta ziņa, ka nav pieejami komentāri
    -	Ja komentāra garums pārsniedz pieļaujamo parametru, tiks izvadīta kļūda.
      
9.	Jānodrošina iespēja pasūtīt bileti. 
    -	Ja lietotājs nav reģistrējies, tad jāizvada poga ar uzrakstu "Reģistrēties".
    -	Ja lietotājs atkārtoti noklikšķina uz "Pasūtīt biļeti", tiks izvadīta ziņa, ka biļets jau ir pasūtīts.
      
10.	Jānodrošina iespēja pievienot jaunas lidojumus adminam.
    -	Ja kāds no laukiem nav ievadīts, izvadīt par to paziņojumu
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam tad tiek izvadīta kļūda.
      
11.	Jānodrošina iespēja pievienot jaunas lidojumus adminam.
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
      
15.	Jānodrošina iespēja pievienot lidojuma  kartes uz galvena ekrana.
    -	Ja kāds no laukiem nav ievadīts, izvadīt par to paziņojumu
    -	Ja kāds no ievadītajiem parametriem neatbilst garumam tad tiek izvadīta kļūda.
    -	Ja profila attēls, kas tika augšupielādēts, ir lielāks par 2 MB, tiks izvadīts paziņojums, ka attēls ir pārāk liels.

## Nefunkcionālās prasības

1.	Mājas lapai jāatbalsta vismaz trīs valodas, ieskaitot latviešu.
2.	Jānodrošina tīmekļa lietojumprogrammas pielāgošanas ekrāna izmēriem, kas mūsdienās tiek lietoti, lai to varētu izmantot uz dažādiem monitora izmēriem.
3.	Dizainam ir jābūt saprotamam un patīkamam lietotājam.
4.	Tekstam jābūt labi redzamam lietotājam un jāizskatās lakoniski kopā ar tīmekļa vietnes noformējumu.
5.	Mājas lapā jābūt instrukcijai par konkrētu darbību veikšanu.
6.	Mājas lapā jābūt iespējai lietotājiem atstāt atsauksmes un komentārus.
7.	Lietotājam profilu jabut saprotamam un ērtam izmantošānā.
8.	Jebkura ievades rinda jāaizsargā pret SQL pieprasījumu ievadi (SQL injekcijām).
9.	Mājaslapai jāstrādā ātri, apstrādājot visu informāciju.
10.	Darbinieka lapai jabut viegli uztvēramai

      
Sistēmas ekrānu skices:
* Galvena lapas skice (skat. 1 att.)

  ![1 att.](https://media.discordapp.net/attachments/1153547180360073270/1210635499891331112/image.png?ex=65eb472b&is=65d8d22b&hm=73fc1855ae5149fdbf9b56b990c828ed119439dab5e7d63f9454dbd9900ac642&=&format=webp&quality=lossless "1 att.")

1.att. Galvena lapas skices attēls 

* Darbinieka lapas skice.  (skat. 2 att.)

  ![2 att.](https://media.discordapp.net/attachments/1153547180360073270/1210635545965756448/image.png?ex=65eb4736&is=65d8d236&hm=4bb23e9f765994425f0e1745028efe655ba372377b68a2ed945edeb9dc0755f0&=&format=webp&quality=lossless&width=834&height=671 "2 att.")

2.att. Darbinieka lapas skices attēls

* Lietotāja komentāru sistēmas skice (skat. 3. att.)

  ![3 att.](https://media.discordapp.net/attachments/1153547180360073270/1210635613041070161/image.png?ex=65eb4746&is=65d8d246&hm=5370b9cb004369ef3aa60e0aedf5f5b316d3d2671f03dffa1e104aab4238cf28&=&format=webp&quality=lossless&width=825&height=671 "3 att.")
 
3.att. Komentāru sistēmas skices attēls
