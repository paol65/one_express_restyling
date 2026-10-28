# One Express: restyling della homepage

Tre proposte grafiche per la homepage di oneexpress.it, pensate per essere ritagliate e applicate al template WordPress ExpeditorBlue. Sono mockup statici: i moduli e i link non funzionano.

| Proposta | Direzione |
|---|---|
| **A · Blu Express** | Hero con modulo di tracciamento, servizi a schede, preventivo, FAQ. |
| **B · Sportello digitale** | Pensata per chi deve fare subito una cosa: tracciare, chiedere un preventivo, trovare la filiale. |
| **C · Il Primo** | Editoriale e scura, con il carattere MicroSquare del marchio. |

## Contenuto del repository

- `index.html`: pagina di presentazione (proposta A/B/C, Desktop/Mobile, menu chiuso/aperto), protetta da password. La password non è in questo repository: chiedila a chi gestisce il progetto.
- `proposte/`: le pagine HTML di ogni proposta.
  - `X-home.html`: homepage responsive con la versione mobile.
  - `X-menu.html`: mega-menu desktop aperti.
  - `Main.html`: panoramica.
  - `img/`: immagini, loghi e font.
- `pdf/`: un PDF lungo per proposta, con desktop menu chiuso, mega-menu aperti, mobile e menu mobile aperto.
- `anteprime/`: screenshot in JPG.
- `LEGGIMI.md`: note per lo sviluppo sul template (blocchi `<!-- EB: … -->`), dati usati e storico delle modifiche.

## Come vederle

Apri `index.html` in un browser, oppure apri direttamente i file in `proposte/`.

Per avere un link pubblico, attiva GitHub Pages: Settings → Pages → Deploy from a branch → `main` / root.

## Da completare prima della pubblicazione

- Segnaposto da sostituire: indirizzo, P.IVA, testimonianze reali.
- Video di Claudio e Andrea Franceschelli: per ora c'è la miniatura con l'icona play.
- Dati ambientali Green Pallet: verificare che corrispondano al report pubblicato (D.Lgs. 30/2026).
