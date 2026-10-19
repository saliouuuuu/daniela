# Daniela Impastato — sito one-page

Sito statico in italiano per Daniela Impastato, consulente d'immagine e personal shopper a Canale (CN).
HTML, CSS e JavaScript scritti a mano: nessun framework, nessuna libreria, nessun cookie.

## Struttura

- `public/index.html`: la pagina (CSS e JS inline)
- `public/privacy.html`: informativa privacy
- `public/assets/img/`: foto in WebP
- `public/assets/fonts/`: Arimo (grotesco in stile Helvetica), ospitato sul sito
- `public/_headers`: intestazioni di sicurezza e cache (Cloudflare)
- `wrangler.jsonc`: dice a Cloudflare di pubblicare solo la cartella `public/`

## Da completare (cercare `DA COMPLETARE` nei file)

- `WA_NUMBER` in fondo a `index.html`: numero WhatsApp senza spazi né prefisso. Finché è vuoto i pulsanti portano al modulo.
- Servizi (titoli, categorie, una riga, foto), "Chi sono", i 4 passi, le 3 recensioni con nome, link alla scheda Google, link Instagram, P.IVA.
- Dominio: `canonical` e Open Graph usano `dominio-da-completare.example`.
- `privacy.html`: titolare (P.IVA, contatti), fornitore di hosting, tempi di conservazione, data.
- `robots.txt`: aggiungere la riga `Sitemap:` quando c'è il dominio.

## Foto

Le foto attuali arrivano da miniature di 179 px di larghezza (raddoppiate): vanno sostituite con gli originali
mantenendo gli stessi nomi di file, o ricreando i WebP alla larghezza che serve (hero almeno 1600 px).

## Pubblicazione

Cloudflare Workers con file statici: collegare il repository, ramo `main`, comando di deploy `npx wrangler deploy`.
