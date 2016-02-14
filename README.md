# Geometria

Questo volume è la trascrizione degli appunti del corso di **Geometria 1** tenuto dal professor Marco Rigoli.
Con il tempo, sono stati integrati anche altri argomenti, tratti dalle lezioni di tutorato o da fonti esterne, per completare il quadro di alcune spiegazioni.
Correzioni e consigli sono *sempre* i benvenuti.

Buona lettura!

### Avvisi
Al momento le dispense coprono le lezioni della primavera del 2014 (A.A. 2013-2014).
Nell'anno successivo il programma del corso ha visto alcune importanti aggiunte, tra cui ricordo:
- approfondimenti (e nuovi teoremi) sulle applicazioni multilineari alternanti;
- il teorema di Cayley-Hamilton, nella forma generale;
- le forme bilineari.
Per ovvi motivi, questi argomenti non sono stati inclusi in queste dispense, ed è poco probabile che lo saranno (da me) in una futura versione; se qualcuno volesse collaborare, in modo da non lasciare scoperto quest'argomento per i futuri lettori, si faccia sentire!

### Informazioni tecniche
##### Struttura dei file
I file `.tex` sono separati per capitolo e si trovano tutti nella cartella `chapters`, e sono inclusi nel file principale con il comando `\include`.

##### Come compilare
Nel menu [releases](https://github.com/phaerrax/geometria/releases) nella barra superiore potete trovare una versione già compilata del documento, che verrà aggiornata di tanto in tanto, oppure in seguito a grossi cambiamenti.
Se volete compilarlo sul vostro computer, in modo da ottenere la versione più aggiornata, ecco i passi da seguire (per una distribuzione Linux con le applicazioni necessarie installate).
I file dei singoli capitoli non possono essere compilati separatamente.
Si consiglia l'uso di `latexmk` per automatizzare i processi di compilazione.

Alla prima compilazione, bisogna generare i file della bibliografia di `biblatex`, perciò serve compilare più volte.
Trovandosi nella cartella principale, eseguire

```bash
pdflatex geometria
biber geometria
pdflatex -shell-escape geometria
pdflatex -shell-escape geometria
```

Le volte successive, se il file `geometria.bib` non è stato modificato e non sono state aggiunte citazioni (in tal caso, ripetere i passaggi precedenti), è sufficiente un unico passaggio:

```bash
pdflatex -shell-escape geometria
```

ripetuto eventualmente una seconda volta per sistemare riferimenti interni.

##### Requisiti
Per poter compilare il documento è necessario ovviamente avere installato tutti i pacchetti di LaTeX elencati nel file di stile e le applicazioni di base per compilare.
Se usate una distribuzione TeX Live per sistemi basati su Debian è sufficiente installare i pacchetti

```
texlive-base
texlive-bibtex-extra
texlive-binaries
texlive-extra-utils
texlive-font-utils
texlive-fonts-recommended
texlive-generic-recommended
texlive-lang-italian
texlive-latex-base
texlive-latex-extra
texlive-latex-recommended
texlive-pictures
texlive-plain-extra
texlive-science
biber
```

