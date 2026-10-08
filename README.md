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
| Pubblicazioni | un file per ciascuna in `_publications/` |
| Convegni e seminari | un file per ciascuno in `_talks/` |
| Didattica | un file per ciascun corso in `_teaching/` |
| Foto | carica in `images/` e scrivi il nome del file in `_config.yml` → `avatar` |
| Voci del menu | `_data/navigation.yml` |

Cerca **`[DA COMPLETARE]`** nei file per trovare tutto quello che manca.

## Come modificare un file dal sito di GitHub

1. Apri il file su github.com e clicca sull'icona della **matita** ✏️ in alto a destra.
2. Modifica il testo.
3. Clicca **Commit changes**. Fatto: dopo 1–2 minuti la modifica è online.

Per caricare un PDF o una foto: apri la cartella (`files/` o `images/`) → **Add file → Upload files**.

## Aggiungere una pubblicazione

1. Apri `_publications/2025-01-01-esempio-articolo.md` e copiane il contenuto.
2. Nella cartella `_publications/` → **Add file → Create new file** e chiamalo ad esempio `2026-03-15-titolo-breve.md`.
3. Incolla il contenuto, compila titolo, data, rivista, DOI e citazione, e **cancella la riga `published: false`**.
4. **Commit changes**.

Interventi (`_talks/`) e didattica (`_teaching/`) funzionano allo stesso modo. Ogni cartella ha il suo file di esempio, che resta nascosto.

Il campo `category` delle pubblicazioni decide in quale sezione compare: `manuscripts` (articoli su rivista), `workingpapers`, `books` (libri e capitoli) o `conferences` (contributi a convegni).

## Se qualcosa non funziona

Nella scheda **Actions** del repository vedi l'esito di ogni ricostruzione del sito. Se compare una ❌, quasi sempre è un errore nelle righe tra i `---` in cima a un file, per esempio una virgoletta non chiusa. Puoi sempre tornare alla versione precedente dalla cronologia del file (**History**).

## Licenza

Template: Academic Pages (MIT), derivato da Minimal Mistakes di Michael Rose. Vedi `LICENSE`.
