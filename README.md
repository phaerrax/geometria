# Geometria

Questo volume è la trascrizione degli appunti del corso di **Geometria 1** dell'A.A. 2013-2014 tenuto dal professor Marco Rigoli.
Con il tempo, sono stati integrati anche altri argomenti, tratti dalle lezioni di tutorato o da fonti esterne, per completare il quadro di alcune spiegazioni.
Correzioni e consigli sono *sempre* i benvenuti.

Buona lettura!

### Avvisi
Come potete vedere, il documento è molto frammentato, e la maggior parte dei capitoli non è ancora terminata: per questo non c'è ancora una versione completa degli appunti.
Nel menu [releases](https://github.com/phaerrax/geometria/releases) potete trovate comunque un "collage" dei vari capitoli (la numerazione dei capitoli e delle pagine potrebbe però essere in disordine).
Il file `geometria.pdf` già presente nella repository è obsoleto e sarà presto eliminato.

Nell'A.A. 2014-2015 il programma del corso ha compreso anche una nuova parte sulle forme bilineari, che per evidenti motivi non è presente in questi appunti.
Al momento è poco probabile che sarà inclusa in una futura versione; se qualcuno volesse collaborare, in modo da non lasciare scoperto quest'argomento per i futuri lettori, si faccia sentire!

### Informazioni tecniche
##### Struttura dei file
I file `.tex` sono separati per capitolo e si trovano tutti nella cartella `chapters`, e sono inclusi nel file principale con `\include`.
Nel *branch* `master` si trovano i capitoli da considerarsi completati.
Per il resto, ogni capitolo ha un *branch* dedicato: la stesura di ogni capitolo avviene così separatamente dal corpo principale, e viene integrato una volta terminato il lavoro.
Se volete dare un'occhiata ai capitoli ancora "*work in progress*" dovete quindi cambiare *branch* nel menu in alto.

##### Come compilare
Se volete compilarlo sul vostro computer, in modo da ottenere la versione più aggiornata, ecco i passi da seguire (per una distribuzione Linux con le applicazioni necessarie installate).
I file dei singoli capitoli non possono essere compilati separatamente.
Si consiglia l'uso di `latexmk` per automatizzare i processi di compilazione.

Trovandosi nella cartella principale, eseguire

```bash
pdflatex geometria
```

un numero sufficiente di volte perché i riferimenti interni siano corretti.

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
texlive-plain-extra
texlive-science
```

