# avai_kasus

Dette repoet er svaret på oppgaven før 2. intervju til AI-teamet hos Arkivverket. Hvis du vil kjøre koden må du først:

* Installere pakkene som er listet opp i requirements.txt (jeg har også listet versjonene jeg har brukt for å sikre at alt kjører som det skal)
* Laste ned spacy-modellen 'nb_core_news_lg'

## Del 1
Del 1 inneholder en relativt enkel OCR-funksjon samt en post-prosessering som tar i bruk enkel stavekontroll for å rette opp i noen av de groveste feilene som kommer med i OCR-resultatet. 

## Del 2
I denne delen har jeg trukket ut innholdsord og gjort en LDA for å finne temaer og temaord i dokumentene. De første cellene av koden i del 2 er delen som leser inn alle dokumentbildene med OCR og lagrer resultatene i mappen 'av_doc_corpus'. Siden det tar ganske lang tid å lese inn alle bildene og hente ut tekst med OCR, anbefaler jeg å bare se på resultatene i mappen, som også er lagt ved. 

Videre i del 2 henter jeg ut innholdsord og gjør en enkel LDA. Deretter lagrer jeg en ny versjon av korpuset i mappen 'av_doc_corpus_keywords', som inneholder alt det samme som i den førstnevnte mappen pluss tokeniserte versjoner av tekstene, innholdsord, temaer (samt score som ble gitt de forskjellige temaene fra LDA-modellen) og temabegreper (ord som "definerer" de forskjellige abstrakte temaene). 
