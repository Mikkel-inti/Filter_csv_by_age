# Filter csv by age
Dette C-program er lavet i forbindelse med kursus: **62712- Basic C-programmeing**. Programmet implementerer filtrering af data fra en CSV-fil baseret på alder, hvor
kun de linjer der opfylder en given maksimumalder beholdes. Denne filtrering kan enten udskrives til en ny CSV-fil eller til terminalen.  
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


### Funktioner
- `filter_stream(FILE *istream, FILE *ostream)`
   -Funktionen filtrerer CSV-linjer fra `istream` baseret på alder og skriver de filtrerede linjer til `ostream`.


## How to use eksempel 
### input(csv) -> output(csv) :

1. Byg programmet ( evt.: `Ctrl Shift B`)
2. Åben terminal og skriv først : .\main
4. Indtast den alder der skal filtres fra: 
   - *Vi vælger: `17`*
5. Indtast din **input .csv-fil** :
   - *Vi vælger: `people-with-age.csv`*
6. Indtast din **output .csv-fil** :
   - *Vi vælger: `out.csv`*

Din fulde terminal skulle nu ligne dette (Tryk enter):
  - `./main.exe 17 people-with-age.csv out.csv`

### input(csv) -> output(terminal) :

1. Byg programmet ( evt.: `Ctrl Shift B`)
2. Åben terminal og skriv først : .\main
4. Indtast den alder der skal filtres fra: 
   - *Vi vælger: `17`*
5. Indtast din **input .csv-fil** :
   - *Vi vælger: `people-with-age.csv`*

Din fulde terminal skulle nu ligne dette (Tryk enter):
  - `./main.exe 17 people-with-age.csv`

### input(terminal) -> output(terminal) :

1. Byg programmet ( evt.: `Ctrl Shift B`)
2. Åben terminal og skriv først : .\main
4. Indtast navn efterfulgt af komma: 
   - *Vi vælger: `Klara,`*
5. Indtast alder :
   - *Vi vælger: `17`*
6. Indtast nu :
   - * `| main.exe`*

Din fulde terminal skulle nu ligne dette (Tryk enter):
  - `Klara, 17 | ./main.exe 17 `
