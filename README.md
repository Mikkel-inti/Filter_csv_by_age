# Filter csv by age
Dette C-program er lavet i forbindelse med kursus: **62712- Basic C-programmeing**. Programmet implementerer filtrering af data fra en CSV-fil baseret på en angivet alder, hvor linjerne der opfylder den angivet maksimumalder, bliver beholdt. Denne filtrering kan enten blive udskreve til en ny CSV-fil eller til terminalen.  
Programmet anvender CLI til at tage:
- en maksimum alder
- en valgfri input-CSV-fil
- en valgfri output-CSV-fil
> **Note:**  
> Er der ikke angivet en input-fil, bliver data læst fra (*stdin*).  
> Er der ikke angivet en output-fil, bliver resultatet til terminalen ( *stdout*).


## Filer
- `main.c` – **Samlede kørsel**, her bestemmes om hvilket in- og output der skal anvendes i filtreringen.
- `people-with-age.csv` - Denne csv fil indeholder forskellige navne og aldre, der kan anvendes til at testkøre programmet.
- `Filter-by-age_flowdia.jpg` - Flow diagram for selve programmet. 


### Funktioner
- `filter_stream(FILE *istream, FILE *ostream)`
   - Funktionen filtrerer CSV-linjer fra `istream` baseret på alder og skriver de filtrerede linjer til `ostream`.


## How to use eksempel 
Ved de to første eksempler hvor input læses fra CSV-fil, bliver der læst fra `people-with-age.csv`. 
Hvor indholdet er:
```
Nuvi Våle, 18

Aeral Körn
Lumio Satō, 29
Veski Ruañ, 12

```
Her vil eksemplerne vise at programmet opfanger at der mangler en linje og en alder. 


### input(csv) -> output(csv) :

1. Byg programmet ( evt.: `Ctrl Shift B`)
2. Åben terminal og skriv først : .\main
3. Indtast den alder der skal filtres fra: 
   - *Vi vælger: `17`*
4. Indtast din **input .csv-fil** :
   - *Vi vælger: `people-with-age.csv`*
5. Indtast den nye **output .csv-fil** :
   - *Vi vælger: `out.csv`*

Din fulde terminal skulle nu ligne dette (Tryk enter):
  - `./main.exe 17 people-with-age.csv out.csv`

#### Eksempel udskrift:
<img width="612" height="92" alt="image" src="https://github.com/user-attachments/assets/76a03d10-5d34-4014-b7c1-83b6cc312b3d" />



### input(csv) -> output(terminal) :

1. Byg programmet ( evt.: `Ctrl Shift B`)
2. Åben terminal og skriv først : .\main
3. Indtast den alder der skal filtres fra: 
   - *Vi vælger: `17`*
4. Indtast din **input .csv-fil** :
   - *Vi vælger: `people-with-age.csv`*

Din fulde terminal skulle nu ligne dette (Tryk enter):
  - `./main.exe 17 people-with-age.csv`
#### Eksempel udskrift:
<img width="443" height="115" alt="image" src="https://github.com/user-attachments/assets/8b076797-cf3e-4a52-bf7d-316e6779b604" />

### input(terminal) -> output(terminal) :

1. Byg programmet ( evt.: `Ctrl Shift B`)
2. Åben terminal og skriv først : .\main
3. Indtast gåseøjne "navn, alder" : 
   - *Vi vælger: `"Klara, 17"`*
4. Indtast nu :
   - * `| main.exe`*

Din fulde terminal skulle nu ligne dette (Tryk enter):
  - ` "Klara, 17" | ./main.exe 17 `

#### Eksempel udskrift:
<img width="384" height="60" alt="image" src="https://github.com/user-attachments/assets/8b5b30be-e387-4d38-a167-a6e581fefefe" />
