# ER-diagramma

![DP41 Deniss Kozlovs ER-diagramma](https://github.com/rvt-prog-kval-24/DP41-DenissKozlovs-AviabiesuMeklesanasUnRezervesanasVietne/blob/main/documentation/atteli/er_diagram.png "DP41 Deniss Kozlovs ER-diagramma")

1.att. Sistēmas ER-modelis

Sistēmas ER-modelis sastāv no 9 entītijām(skat 1. att.), kas nodrošina pamat informācijas uzglabāšanu un apstrādi. Tie ir: 
* “Pieejamais datums” – šī entītija parāda visus pieejamos datumus, kurus var rezervēt konkrētiem lidojumiem, un cenas konkrētiem datumiem. Katram datumam ir savs unikāls ID.
* “lidostas/avialīnijas” – šī entītija parāda detalizētu informāciju par lidojumu. Katram lidojumam ir savs unikāls ID. 
* “lidojuma apraksts” – šī entītija parāda lidojuma aprakstu. Katram aprakstam ir savs unikāls ID.
* “Profila attēli” – šī entītija parāda profila attēlu . Katram attēlam ir savs unikāls ID.
* “lietotāji” – šī entītija parāda detalizētu informāciju par lietotāju. Katram lietotājam ir unikāls ID.
* “komentāri” – šī entītija parāda katra lietotāja komentārus. Katram komentāram ir savs unikāls ID. 
* “Bērni” – šī entītija parāda visus bērnus, viņas personas dati un cenas par sēdvietu. Katram bernam ir savs ID.
* “Biļetes” – šī entītija ir saistītā tabula, kurā ir tikai pievienoto tabulu ID.
* “Lietotāja informācija” – šī entītija parāda lietotāja personiskie dati. Katrai datu rindai ir savs ID.
