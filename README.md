# WWII Letters Suite

Suite statica per l'esplorazione del corpus **Ultime lettere della Seconda guerra mondiale**.

Contiene tre ambienti principali:

- **Mappa geospaziale** (`letters_geospatial_leaflet_v2.html`)
- **Lexicon** (`letters_nlp_lexicon.html`)
- **Links + trends** (`letters_nlp_lexicon_links_trends.html`)
- **Hub di accesso** (`index.html`)

## Link: https://digitalkoine.github.io/lastlettersfirstdb/

## Struttura dei file

```text
.
├── index.html
├── letters_geospatial_leaflet_v2.html
├── letters_geospatial_leaflet_v2.geojson
├── letters_geospatial_leaflet_v2.xlsx
├── letters_nlp_lexicon.html
├── letters_nlp_lexicon.xlsx
├── letters_nlp_lexicon_links_trends.html
└── README.md
```

## Uso locale

1. Scarica o clona la cartella.
2. Mantieni tutti i file nella stessa directory.
3. Apri `index.html` nel browser.

Per un uso più stabile, è consigliabile servire la cartella con un piccolo server locale.

Esempio con Python:

```bash
python3 -m http.server 8000
```

Poi apri il browser su:

```text
http://localhost:8000/
```

## Pubblicazione su GitHub Pages

### Opzione semplice: repository dedicato

1. Crea un nuovo repository su GitHub.
2. Carica **tutti** i file della cartella nella root del repository.
3. Vai in **Settings → Pages**.
4. In **Build and deployment**, scegli:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (o `master`)
   - **Folder**: `/ (root)`
5. Salva.

Dopo qualche istante il sito sarà pubblicato su GitHub Pages.

## Avvio consigliato

La pagina iniziale da pubblicare è:

```text
index.html
```

## Note importanti

- Non rinominare i file HTML o i file dati, perché i collegamenti interni dipendono da quei nomi.
- Il file `letters_geospatial_leaflet_v2.html` può dipendere dalla disponibilità dei tile di base della mappa.
- Se qualcosa non si vede correttamente aprendo i file con doppio clic, prova con un server locale o con GitHub Pages.

## Suggerimento per il repository

Puoi aggiungere anche un file `.gitignore` minimo come questo:

```gitignore
.DS_Store
__MACOSX/
```

## Licenza e crediti

Aggiungi qui i crediti scientifici, le fonti del corpus e l'eventuale licenza di riuso dei materiali.
