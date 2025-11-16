# Filter csv by age
Dette C-program er lavet i forbindelse med kursus: **62712- Basic C-programmeing**, 

## Filer
- `main.c` – **Samlede kørsel**, her bestemmes om hvilket in- og output der skal anvendes i filtreringen.
- `people-with-age.csv` - Denne csv fil indeholder forskellige navne og aldre, der kan anvendes til at testkøre programmet. 


### Funktioner
- `filter_stream(FILE *istream, FILE *ostream)`
- Funktionen læser linje for linje fra `istream`( enten en .csv-fil eller standard input ).


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
