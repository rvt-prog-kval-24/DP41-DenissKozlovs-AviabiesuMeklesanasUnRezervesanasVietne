# DATU STRUKTŪRAS APRAKSTS
Datu bāze sastāv no 9 tabulām, kurās ir informācija par lietotāju, katru lietotāja komentāru, lietotāja pasūtījumiem, aviokompānijas informāciju un biļetēm. Zemāk ir attēlota tabulu attiecību shēma (Skat.2 attēlu).
●	Tabulā "airports/airlines" tiek glabāti dati par lidojumiem. 
●	Tabulā "tickets" tiek glabāti dati par biļetēm. 
●	Tabulā "children" tiek glabāti dati par lietotāja bērniem. 
●	Tabulā "users" tiek glabāti dati par lietotājiem. 
●	Tabulā "comments" tiek glabāti dati par lietotāja komentāriem. 
●	Tabulā "profile_images" tiek glabāti dati par lietotāja profila attēliem. 
●	Tabulā "user_details" tiek glabāta lietotāju personiskā informācija.
●	Tabulā "acessabledata" tiek glabāta informācija par konkrētajām datumām un laikā pieejamam lidojumam.
●	Tabulā "airflight_description" tiek glabāta informācija par lidojumu aprakstu.
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
