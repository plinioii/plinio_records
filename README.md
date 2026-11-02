# Plinio Records – Collezione e Wantlist (PWA)

Dashboard della collezione e della wantlist Discogs, installabile come app su telefono e computer
e utilizzabile anche offline.

## Pubblicazione su GitHub Pages
1. Crea un repository su GitHub (es. `plinio-records`).
2. Carica **tutto il contenuto di questa cartella** nella radice del repository
   (`index.html`, `manifest.webmanifest`, `sw.js`, `.nojekyll`, cartelle `icons/` e `data/`).
   Dal sito: *Add file › Upload files*, trascina i file e fai *Commit*.
3. Vai in *Settings › Pages*: Source = *Deploy from a branch*, Branch = `main`, cartella `/ (root)`, *Save*.
4. Dopo un minuto l'app è su `https://<tuo-utente>.github.io/plinio-records/`.

## Installazione
- **Android (Chrome)**: apri il link, menu ⋮ › *Installa app* (o *Aggiungi a schermata Home*).
- **iPhone (Safari)**: tasto Condividi › *Aggiungi alla schermata Home*.
- **PC (Chrome/Edge)**: icona di installazione nella barra degli indirizzi.

## Dati
- Dentro l'app usa **Carica CSV** su Collezione e Wantlist (export da Discogs › Esporta).
  Il file resta salvato su quel dispositivo, con data e ora del caricamento.
- In alternativa metti `collection.csv` e `wantlist.csv` nella cartella `data/` del repository:
  l'app li carica da sola dove non è stato caricato nulla a mano.
  Attenzione: in un repository pubblico quei file (note comprese) sono scaricabili da chiunque.

## Aggiornare l'app
Dopo aver modificato i file, cambia `VERSION` in `sw.js` (es. `plinio-v2`)
così i dispositivi scaricano la nuova versione.
