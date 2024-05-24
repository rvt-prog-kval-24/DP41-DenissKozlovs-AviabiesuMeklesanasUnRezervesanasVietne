# Funkcionālas dekompozīcijas diagramma
## Sistēmas struktūras modelis
### Sistēmas arhitektūra
Sistēmu veido četras apakšsistēmas: biļešu datu apstrādes, personas konta datu apstrāde, filtrēšanas datu apstrāde, lietotāja datu apstrāde. (skat. 1. att.)

![DP41 Deniss Kozlovs Funkcionālas dekompozīcijas diagramma](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/funkc_dekomp_diagram.png "DP41 Deniss Kozlovs Funkcionālas dekompozīcijas diagramma")

1.att. Funkcionālās dekompozīcijas diagramma


*	Aviabiļešu datu apstrādes apakšsistēma ir atbildīga par datiem par visām aviobiļetēm, ko administrators ir izveidojis un pievienojis datu bāzei. Šī apakšsistēma ļauj pievienot, dzēst, rediģēt, apmaksāt un izdrukāt biļetes.

*	Personas konta datu apstrādes apakšsistēma ir atbildīga par visu informāciju par konkrētas sesijas lietotāju. Šī apakšsistēma ļauj rediģēt konkrētas sesijas lietotāja paroli, vārdu, attēlu, kā arī apskatīt un anulēt rezervētās biļetes.

*	Filtrēšanas datu apstrādes apakšsistēma ir atbildīga par meklēšanas rindā ievadīto datu filtrēšanu un turpmāko filtrēšanas rezultātu izvadīšanu.  Šī apakšsistēma ļauj filtrēt un meklēt informāciju pēc pieprasījuma, kā arī apstrādāt ievadītos datus filtrēšanai.

*	Lietotāju datu apstrādes apakšsistēma ir atbildīga par datu apstrādi par visiem sistēmā reģistrētajiem vai autorizētajiem lietotājiem. Šī apakšsistēma ļauj apstrādāt lietotāju reģistrācijas un autorizācijas datus, kā arī pārbaudīt datus attiecībā uz rakstzīmju garumu, rakstzīmju atļaujām utt. 
