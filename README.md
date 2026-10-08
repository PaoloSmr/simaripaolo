# Sito accademico di Paolo Simari

Il sito è costruito con il template [Academic Pages](https://github.com/academicpages/academicpages.github.io) ed è pubblicato gratis con GitHub Pages. Non ci sono plugin da aggiornare né server da mantenere: ogni volta che salvi una modifica in questo repository, GitHub ricostruisce il sito da solo in 1–2 minuti.

Indirizzo: **https://paolosmr.github.io/simaripaolo**

## Metterlo online (una volta sola)

1. Nel repository vai su **Settings → Pages**.
2. In *Build and deployment* scegli **Source: Deploy from a branch**, poi **Branch: `main`** e cartella **`/ (root)`**, e premi **Save**.
3. Dopo un paio di minuti il sito è all'indirizzo qui sopra.

> **Facoltativo: indirizzo più corto.** Rinomina il repository in `paolosmr.github.io` (Settings → General → Repository name). Poi in `_config.yml` imposta `baseurl: ""`. Il sito sarà su `https://paolosmr.github.io`.

## Dove si modifica cosa

| Cosa | File |
|---|---|
| Nome, bio breve, università, email, link a Scholar/ORCID/LinkedIn | `_config.yml` (sezione `author`) |
| Testo della home | `_pages/about.md` |
| CV | `_pages/cv.md` + il PDF in `files/cv.pdf` |
| Ricerca (working paper, pubblicazioni, dataset) | un file per ciascuno in `_publications/` |
| Convegni e seminari | un file per ciascuno in `_talks/` |
| Didattica | un file per ciascun corso in `_teaching/` |
| Foto | carica in `images/` e scrivi il nome del file in `_config.yml` → `avatar` |
| Voci del menu | `_data/navigation.yml` |

## Come modificare un file dal sito di GitHub

1. Apri il file su github.com e clicca sull'icona della **matita** ✏️ in alto a destra.
2. Modifica il testo.
3. Clicca **Commit changes**. Fatto: dopo 1–2 minuti la modifica è online.

Per caricare un PDF o una foto: apri la cartella (`files/` o `images/`) → **Add file → Upload files**.

## Aggiungere una pubblicazione

1. Apri una pubblicazione già presente in `_publications/` (ad esempio `2026-08-24-stanze-ascolto-femminicidi.md`) e copiane il contenuto.
2. Nella cartella `_publications/` → **Add file → Create new file** e chiamalo ad esempio `2027-03-15-titolo-breve.md`.
3. Incolla il contenuto e cambia titolo, data, rivista e testo. Se vuoi, aggiungi `paperurl: "https://doi.org/..."` (link al paper) e `citation: '...'` (citazione completa).
4. **Commit changes**.

Didattica (`_teaching/`) funziona allo stesso modo. Per i convegni in cui presenti un lavoro c'è un modello nascosto in `_talks/`: copialo, cancella la riga `published: false` e aggiungi la voce "Interventi" al menu in `_data/navigation.yml`.

Il campo `category` decide in quale sezione della pagina Ricerca compare: `manuscripts` (articoli su rivista), `workingpapers`, `workinprogress` (lavori in corso), `datasets`, `books` (libri e capitoli) o `conferences` (contributi a convegni). Quando un working paper viene pubblicato, basta cambiare `category` in `manuscripts` e `venue` con il nome della rivista.

La riga `hide_year: true` nasconde l'anno (utile quando non è ancora definito).

**Aggiornare il CV:** sostituisci `files/cv.pdf` (Upload files, stesso nome). Ricordati di usare una versione **senza** codice fiscale, indirizzo di casa e telefono.

## Se qualcosa non funziona

Nella scheda **Actions** del repository vedi l'esito di ogni ricostruzione del sito. Se compare una ❌, quasi sempre è un errore nelle righe tra i `---` in cima a un file, per esempio una virgoletta non chiusa. Puoi sempre tornare alla versione precedente dalla cronologia del file (**History**).

## Licenza

Template: Academic Pages (MIT), derivato da Minimal Mistakes di Michael Rose. Vedi `LICENSE`.
