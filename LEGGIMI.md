# One Express – nuova homepage, 3 proposte (ottobre 2026)

Canvas con tutte le tavole: https://claude.ai/artifact/7FD7pWcbucX5MG3q1vM5bU

## File
| File | Contenuto |
|---|---|
| `Main.html` | Brief, logo su due righe, palette, mappa blocchi → template |
| `A-home.html` / `A-menu.html` | Proposta A «Blu Express»: homepage con menu chiusi / mega-menu aperti |
| `B-home.html` / `B-menu.html` | Proposta B «Sportello digitale» |
| `C-home.html` / `C-menu.html` | Proposta C «Il Primo» (usa MicroSquare Bold Italic, in `img/`) |
| `img/` | Foto ridimensionate (1800 px), logo su due righe senza payoff, loghi Formula |
| `anteprime/` | Screenshot a pagina intera di ogni tavola |

Ogni homepage contiene già nel `<head>` lo schema **Organization + FAQPage** (JSON-LD) generato dalle FAQ in pagina e una meta description.

## Come ritagliare per ExpeditorBlue (homepage-2)
Ogni sezione è preceduta da un commento `<!-- EB: … -->` con il nome del blocco del template e ha una classe `oe-*`:

- `.oe-topbar` → Top bar
- `.oe-header` / `.oe-mega` → Header e mega menu (Elementor/menu del tema)
- `.oe-hero` → Slider/hero con modulo tracking
- `.oe-quick` → Feature boxes
- `.oe-services`, `.oe-about`, `.oe-stats`, `.oe-process` → Services, About, Counters, Work process
- `.oe-quote` → Request a quote (Contact Form 7)
- `.oe-sectors`, `.oe-green`, `.oe-testimonials`, `.oe-faq`, `.oe-news`, `.oe-footer`

Il CSS di ogni proposta è tutto nel `<style>` in testa al file, con variabili colore (`--blu`, `--scuro`, `--giallo`…) da copiare nel CSS aggiuntivo del tema.

## Da completare prima della messa online
- Segnaposto tra parentesi quadre: numero assistenza, indirizzo, P.IVA, tempo di risposta preventivi, link social.
- Testimonianze: le foto sono persone reali della library; le citazioni sono segnaposto da sostituire con frasi vere (rubrica «L'Eccellenza del Territorio»).
- Descrizioni brevi delle Formule (Silver, Gold, ecc.): da validare con il commerciale.
- Numeri usati (fonte: documento «Posizionamento Strategico» e Brand Book): 139 affiliati, 13.000 bancali/giorno, 3 hub, 41 paesi europei (senza citare partner), 655 MWh e 193 tCO₂eq (2024), dal 2008.

## Aggiornamento 27/10/2026
- Anno di fondazione corretto: 2008.
- Rimossa la citazione dell'alleanza europea: resta solo il dato "41 paesi".
- New One, New Way usa la foto drone «ONE» (img/new-one-new-way-drone.jpg).
- Nessuna foto ripetuta nella stessa proposta (homepage + mega-menu).

## Aggiornamento 27/10/2026: testi Green Pallet e D.Lgs. 30/2026

Testi ambientali riscritti per il D.Lgs. 30/2026, che recepisce la direttiva (UE) 2024/825 ed è in vigore dal 27/09/2026.
- Tolti i claim generici o non dimostrabili: "pesa meno sul pianeta", "più leggeri sul pianeta", "hub alimentati dal sole" e la promessa che scegliere One Express riduce lo Scope 3 del cliente.
- Ogni numero ora ha anno, perimetro ("impianti fotovoltaici dei nostri hub") e una nota con la fonte (Report di sostenibilità 2024). La CO₂ è indicata come "stimata come evitata".
- "Legno certificato" è diventato "legno a standard EPAL", perché non era indicata la certificazione.
- Nei menu, "Sostenibilità" è diventato "Dati ambientali". La CTA ora è "Leggi dati e metodo".
- Da verificare prima della pubblicazione: che il report pubblicato contenga i dati e il metodo, e il nome "Green Pallet" (vedi nota nel thread).

## Aggiornamento 27/10/2026: versione mobile, PDF e pagina di presentazione

- Le tre home (`A/B/C-home.html`) sono responsive. Sotto gli 860px mostrano:
  - un header mobile con logo, lente "Traccia" e hamburger;
  - un menu off-canvas a fisarmonica con accesso rapido a Traccia, Preventivo, Filiale e Tempi;
  - lingue, telefono e area clienti in fondo al menu;
  - una barra azioni fissa in basso (Traccia, Preventivo, Filiale).
- Lo schema è quello del menu mobile di ExpeditorBlue/Elementor: Header mobile > Off-canvas > Nav menu in modalità dropdown/accordion. I blocchi sono marcati `<!-- EB: Header mobile -->` e `<!-- EB: Barra azioni mobile -->`, con CSS in `<style id="oe-mobile">`.
- Correzioni solo mobile:
  - testimonianze e news in carosello a scorrimento;
  - in B, la tabella comparativa diventa a schede e i filtri scorrono in orizzontale;
  - in C, la lista dei servizi è compattata;
  - immagini Green Pallet più basse;
  - footer su due colonne.
- Stati apribili da URL: `#menu` (menu aperto), `#menu-servizi` (menu aperto su Servizi), `#menu-all` (tutte le voci aperte).
- `pdf/`: un PDF lungo per proposta, con 4 pagine: desktop con menu chiuso, mega-menu desktop aperti, mobile, menu mobile con tutte le voci aperte.
- `anteprime/`: aggiunte le anteprime mobile e del menu mobile.

## Aggiornamento 27/10/2026: box video nelle news

- Nelle news di A, B e C il 2° e il 3° box sono i video di Claudio e Andrea Franceschelli. Per ora c'è la foto con l'icona play e l'etichetta "Video", perché i video sono ancora da produrre.
- Claudio: "I traguardi del 2026" / **Un anno di grandi successi: contro ogni previsione...**
- Andrea: "Gli obiettivi del 2027" / **Sarà un anno di importantissime sfide: le novità del 2027...**
- Immagini: `img/video-claudio-franceschelli.jpg` e `img/video-andrea-franceschelli.jpg`. Quando i video saranno pronti, nel template il box diventa un widget Video di Elementor (YouTube/Vimeo o file) con questa foto come immagine di copertina.
