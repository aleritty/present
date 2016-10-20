# ALERITTY'S DESK.JS

Questo è il sistema che utilizzo per craere le mie presentazioni.

Non è perfetto e richiede la conoscenza come minimo di una base di HTML e preferibilmente di CSS per creare le proprie presentazioni.

Ogni presentazione può poi diventare un eseguibile indipendente, utilizzabile online o offline su qualsiasi computer dotato di un browser moderno.

## Primi step

E' sufficiente scaricare l'archivio o clonare il repository, installare jekyll tramite il proprio metodo preferito e lanciarlo con `jekyll serve`

Per creare le proprie slide basta salvarle nella cartella `_slides`, una per file (solo il contenuto)
il nome del file determina l'ordine ed il titolo (che deve essere univoco).

Le immagini potete caricarle nella cartella `img` e potete far riferimento nella slide con `{{ site.url }}{{ site. baseurl }}/img/NOMEIMMAGINE` ricordate di calibrare la dimensione in base a dove proietterete.

In seguito:
* Compilare il file `_config.yml` con i propri dati
* scegliere un tema per le slide tra quelli contenuti in `assets/themes/style`  
  oppure creare il proprio e piazzarlo li
* scegliere un tema per le transizioni tra quelli contenuti in `assets/themes/transition`  
  oppure creare il proprio e piazzarlo li
* abilitare o disabilitare i plugin che si vogliono utilizzare (se non danno fastidio potete lasciarli, la presentazione è comunque decisamente più leggera che con powerpoint)

Se avete modifiche o create altri stili potete segnalarmeli aprendo una issue o una pull-request su github.

## Comandi
#### Durante la presentazione

Le slide scorrono secondo la transizione scelta utilizzando le frecce.  
Ho disattivato volontariamente la rotellina del mouse.

#### Estensioni

* menu --> `m` mostra la panoramica delle slide
* goto --> `g` mostra il menu per spostarsi nelle slide
* scale --> `s` dovrebbe cambiare qualcosa nella scala dell slide...
* blank --> `.` o `w` nascondono il contenuto attuale
* zoom --> abilita `HOME`, `END`, `b`ookmark e `r`eturn (to bookmark)
* search --> `f` mostra la finestra di ricerca testuale


## TODO

* favicon
* migliora gli stili di automatic
* migliora gli stili di search
* migliora jekyll
  * copia solo i file selettivamente attivati
  * boh, ottimizza
* configura dal file config.yml
* crea/trova i plugin mancanti o falli funzionare
  * note
  * timer
  * presenter console
* Scrivi una buona guida
* crea un eseguibile o similare con:
  * `python -m SimpleHTTPServer`
  * `jekyll serve` oppure `build` (con file di installazione?)
  * lo script (sh + bat?) lancia il browser a localhost:4000
