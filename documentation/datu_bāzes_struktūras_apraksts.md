# DATU STRUKTŪRAS APRAKSTS
Datu bāze sastāv no 9 tabulām, kurās ir informācija par lietotāju, katru lietotāja komentāru, lietotāja pasūtījumiem, aviakompānijas informāciju un biļetēm. "er_diagramma.md" ir attēlota tabulu attiecību shēma (Skat.14 attēlu).
*	Tabulā "airports/airlines" tiek glabāti dati par lidojumiem. 
*	Tabulā "tickets" tiek glabāti dati par biļetēm. 
*	Tabulā "children" tiek glabāti dati par lietotāja bērniem. 
*	Tabulā "users" tiek glabāti dati par lietotājiem. 
*	Tabulā "comments" tiek glabāti dati par lietotāja komentāriem. 
*	Tabulā "profile_images" tiek glabāti dati par lietotāja profila attēliem. 
*	Tabulā "user_details" tiek glabāta lietotāju personiskā informācija.
*	Tabulā "acessabledata" tiek glabāta informācija par konkrētajām datumām un laikā pieejamam lidojumam.
* Tabulā "airflight_description" tiek glabāta informācija par lidojumu aprakstu.

Tabula “airports/airlines” ir saistīta ar tabulam “airflight_description”,“tickets” un “acessabledata”.

1.Tabula
Tabulas “airports/airlines” struktūra


| Nr. | Nosaukums         | Tips      | Garums | Apraksts                                      |
|-----|-------------------|-----------|--------|-----------------------------------------------|
| 1   | id                | int       | 11     | lidojuma identifikācijas numurs(Primārā atslēga) |
| 2   | Airline           | varchar   | 255    | lidojuma nosaukums                            |
| 3   | airport_name      | varchar   | 255    | Lidostas nosaukums                            |
| 4   | ITADA             | varchar   | 3      | ITADA kods                                    |
| 5   | City              | varchar   | 255    | Ierašanās pilsētas nosaukums                  |
| 6   | country           | varchar   | 255    | Ierašanās valsts nosaukums                    |
| 7   | T_price           | varchar   | 8      | Biļēšu cena                                   |
| 8   | arrival_date      | date      | -      | Lidmašīnas ierašanās datums                   |
| 9   | departure_date    | date      | -      | Lidmašīnas iziešanas datums                   |
| 10  | arrival_time      | time      | -      | Lidmašīnas ierašanās laiks                    |
| 11  | departure_time    | time      | -      | Lidmašīnas iziešanas laiks                    |
| 12  | googleMapsLink    | varchar   | 1000   | Saite uz konkrētu vietu Google Kartēs         |
| 13  | created_at        | datetime  | -      | Automatiski izveidots datums un laiks         |


Tabula “tickets” ir saistīta ar tabulam “airports/airlines” un “users”.

2.Tabula
Tabulas “tickets” struktūra

| Nr. | Nosaukums   | Tips    | Garums | Apraksts                                         |
|-----|-------------|---------|--------|--------------------------------------------------|
| 1   | ticket_id   | int     | 10     | Biļetes identifikācijas numurs. (Primārā atslēga)|
| 2   | user_id     | int     | 11     | Lietotāja identifikācijas numurs. (Ārēja atslēga)|
| 3   | airlines_id | int     | 11     | lidojuma identifikācijas numurs. (Ārēja atslēga) |
| 4   | Seat        | varchar | 5      | Sēdvietas numurs                                 |
| 5   | price       | varchar | 10     | Biļetes cena                                     |
| 6   | condition   | varchar | 10     | Biļetes stāvoklis                                |
| 7   | code        | varchar | 12     | Biļetes kods                                     |


Tabula “children” ir saistīta ar tabulam “airports/airlines” un “users”.

3.Tabula
Tabulas “children” struktūra

| Nr. | Nosaukums               | Tips    | Garums | Apraksts                                   |
|-----|-------------------------|---------|--------|--------------------------------------------|
| 1   | children_id             | int     | 11     | Bērna identifikācijas numurs. (Primārā atslēga) |
| 2   | user_id                 | int     | 11     | Lietotāja identifikācijas numurs. (Ārēja atslēga) |
| 3   | airline_id              | int     | 11     | lidojuma identifikācijas numurs. (Ārēja atslēga) |
| 4   | Name                    | varchar | 255    | Bērna vārds                                |
| 5   | Surname                 | varchar | 255    | Bērna uzvārds                              |
| 6   | Nationality             | varchar | 255    | Bērna pilsonība                            |
| 7   | Passport_number         | varchar | 255    | Bērna pases numurs                         |
| 8   | Gender                  | varchar | 255    | Bērna dzimums                              |
| 9   | passportIssuedDate      | date    | -      | Pases izsniegšanas datums                  |
| 10  | passportExpirationDate  | date    | -      | Pases derīguma termiņš                     |
| 11  | seat                    | varchar | 4      | Sēdvietas numurs                           |
| 12  | seatprice               | varchar | 5      | Sēdvietas cena                             |


Tabula “users” ir saistīta ar tabulam “comments”, “children”,”tickets” , “user_details” un “profile_images”.

4.Tabula
Tabulas “users” struktūra

| Nr. | Nosaukums   | Tips    | Garums | Apraksts                                   |
|-----|-------------|---------|--------|--------------------------------------------|
| 1   | user_id     | int     | 11     | Lietotāja identifikācijas numurs. (Primārā atslēga) |
| 2   | username    | varchar | 255    | Lietotāja vārds                            |
| 3   | email       | varchar | 255    | Lietotāja e-pasta adrese                   |
| 4   | password    | varchar | 128    | Lietotāja parole                           |
| 5   | created_at  | datetime| -      | Konta izveides datums un laiks             |

Tabula “comments” ir saistīta ar tabulu “users”.

5.Tabula
Tabulas “comments” struktūra

| Nr. | Nosaukums          | Tips    | Garums | Apraksts                                   |
|-----|--------------------|---------|--------|--------------------------------------------|
| 1   | id                 | int     | 11     | Komentāra identifikācijas numurs. (Primārā atslēga) |
| 2   | name               | varchar | 255    | Komentētāja vārds                          |
| 3   | email              | varchar | 255    | Komentētāja e-pasta adrese                 |
| 4   | comment            | text    | -      | Komentāra saturs                           |
| 5   | created_at         | datetime| -      | Komentāra izveides datums un laiks         |
| 6   | user_id            | int     | 11     | Lietotāja identifikācijas numurs. (Ārēja atslēga) |
| 7   | comment_category   | varchar | 255    | Komentāra kategorija                       |


Tabula “profile_images” ir saistīta ar tabulu “users”.

6.Tabula
Tabulas “profile_images” struktūra

| Nr. | Nosaukums    | Tips      | Garums | Apraksts                                            |
|-----|--------------|-----------|--------|-----------------------------------------------------|
| 1   | profile_image| longblob  | -      | Lietotāja profila attēls                            |
| 2   | id           | int       | 255    | Profila attēla identifikācijas numurs. (Primārā atslēga) |
| 3   | user_id      | int       | 11     | Lietotāja identifikācijas numurs. (Ārēja atslēga)   |
| 4   | image_type   | varchar   | 255    | Profila attēla veids                                |


Tabula “user_details” ir saistīta ar tabulu “users”.

7.Tabula
Tabulas “user_details” struktūra


| Nr. | Nosaukums                     | Tips     | Garums | Apraksts                                                  |
|-----|-------------------------------|----------|--------|-----------------------------------------------------------|
| 1   | details_id                    | int      | 10     | Detalizētas informācijas identifikācijas numurs. (Primārā atslēga) |
| 2   | user_id                       | int      | 11     | Lietotāja identifikācijas numurs. (Ārēja atslēga)         |
| 3   | Name                          | varchar  | 255    | Lietotāja vārds                                            |
| 4   | Surname                       | varchar  | 255    | Lietotāja uzvārds                                          |
| 5   | Gender                        | varchar  | 10     | Lietotāja dzimums                                          |
| 6   | Nationality                   | varchar  | 255    | Lietotāja pilsonība                                        |
| 7   | Phone_number                  | varchar  | 15     | Lietotāja tālruņa numurs                                   |
| 8   | Passport_number               | varchar  | 15     | Lietotāja pases numurs                                     |
| 9   | Passport_issued_date          | date     | -      | Pases izdošanas datums                                     |
| 10  | Passport_expiration_date      | date     | -      | Pases derīguma termiņš                                     |
| 11  | Issued_country_passport       | varchar  | 255    | Valsts, kurā pase tika izdota                             |
| 12  | created_at                    | datetime | -      | Izveides datums un laiks                                   |

Tabula “acessabledata” ir saistīta ar tabulu “airports/airlines”.

8.Tabula
Tabulas “acessabledata” struktūra

| Nr. | Nosaukums       | Tips     | Garums | Apraksts                                                      |
|-----|-----------------|----------|--------|---------------------------------------------------------------|
| 1   | id              | int      | 5      | lidojuma pieejamības datu identifikācijas numurs. (Primārā atslēga) |
| 2   | airline_id      | int      | 11     | lidojuma identifikācijas numurs. (Ārēja atslēga)          |
| 3   | departure_date  | date     | -      | Izlidošanas datums                                             |
| 4   | arrival_date    | date     | -      | Ierašanās datums                                               |
| 5   | departure_time  | time     | -      | Izlidošanas laiks                                              |
| 6   | arrival_time    | time     | -      | Ierašanās laiks                                                |
| 7   | price           | varchar  | 5      | Biļetes cena                                                   |

Tabula “airflight_description” ir saistīta ar tabulu “airports/airlines”.

9.Tabula
Tabulas “airflight_description” struktūra

| Nr. | Nosaukums       | Tips     | Garums | Apraksts                                                      |
|-----|-----------------|----------|--------|---------------------------------------------------------------|
| 1   | description_id  | int      | 5      | Lidojuma apraksta identifikācijas numurs. (Primārā atslēga)   |
| 2   | description     | varchar  | 11     | Lidojuma apraksts.                                         |
| 3   | flight_image    | longblob | -      | Lidojuma attēls                                           |
| 4   | flight_id       | int      | -      | Lidojuma identifikācijas numurs. (Ārēja atslēga)              |



Dati fiziskajā līmenī tiek strukturizēti un uzglabāti, izmantojot shēmu ar saitēm (skat. 13. attēlu). Šāda struktūra nodrošina ērtu un efektīvu datu uzglabāšanu, tāpat šāda struktūra ļauj ietaupīt vietu tabulās, kas savukārt samazina sistēmas slodzi.

![DP41 Deniss Kozlovs Datubāzes_fiziskās_struktūras_shēma](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/Datubāzes_fiziskās_struktūras_shēma.png "DP41 Deniss Kozlovs Datubāzes_fiziskās_struktūras_shēma")

13.att Datubāzes fiziskās struktūras shēma
