# Plan de antrenament — 12 săptămâni

Aplicație web într-un singur fișier pentru un program de forță de 12 săptămâni, cu un plan
de alergare de 52 de săptămâni, meniu pe 7 zile și urmărirea obiceiurilor zilnice.

**[Deschide aplicația →](https://fluxbitz.github.io/gym-planV2/)**

## Ce conține

| Tab | Ce face |
|---|---|
| **Antrenament** | 12 săptămâni × 5 zile, 6 exerciții pe zi. Greutate recomandată calculată per exercițiu, cronometru de pauză, bifare pe serii, încălzire și rutină de recuperare pentru coloană. |
| **Alergare** | Progresie „return to run" pe 52 de săptămâni până la 5 km continuu, cu viteza și panta exacte de bandă pentru fiecare săptămână. |
| **Meniu** | 7 zile × 3 mese, cu gramaje și ore. Acoperirea micronutrienților din alimente, fără suplimente. |
| **Obiceiuri** | 5 obiceiuri zilnice, serie de 7 zile, plus programul plimbărilor pentru 10.000 de pași. |

## Cum se folosește

Deschide `index.html` — nu are nevoie de build, server sau dependențe. La prima deschidere îți
cere datele (vârstă, înălțime, greutate, greutate țintă) și își calculează singură țintele
calorice, de proteină și ritmul de slăbire.

**Datele tale rămân în `localStorage`, pe dispozitivul tău.** Nu există server, nu pleacă nimic
nicăieri, iar în cod nu e scris nimic personal.

## Cum e construit

Un singur `index.html`, fără dependențe. Cele 12 săptămâni de antrenament nu sunt scrise de
mână — se generează dintr-o bibliotecă de exerciții (`EX`), trei șabloane de fază (`PHASES`)
și o schemă săptămânală (`WEEK_SCHEME`), astfel încât o modificare într-un șablon se propagă
în tot programul.

Exercițiile sunt mapate pe aparate HOIST Fitness, fiecare cu link către producător, video de
execuție și o variantă alternativă cu gantere sau kettlebell.

## Adaptări pentru articulații sensibile

Programul e construit pentru cineva cu probleme de genunchi, șold și nerv sciatic:

- fără genuflexiuni cu bară, îndreptări, alergare sau sărituri
- leg press cu amplitudine oprită la 90°, leg extension doar între 90° și 30°
- extensii lombare parțiale, core pe antirotație în loc de rotație
- încălzire complet fără impact
- rutină zilnică de recuperare pentru coloană și sciatic
- alergarea începe abia în săptămâna 13, după ce scade greutatea și crește forța

Nu e sfat medical. Dacă ai dureri articulare, mergi întâi la un specialist.
