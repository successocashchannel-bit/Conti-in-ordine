# Conti in ordine

App web (PWA) per registrare entrate e uscite e pianificare il rientro dai debiti.
Un solo file `index.html`, nessun server, nessuna dipendenza esterna. I dati restano nel browser dell’utente.

## Pubblicarla
Carica l’intera cartella su un hosting statico con HTTPS (Cloudflare Pages, Netlify, GitHub Pages, un normale hosting web).
L’utente apre il link e la aggiunge alla schermata Home: si installa come un’app e funziona anche offline.

## Cosa cambiare prima di venderla
- Nome e icona: `index.html` (titolo e testo), `manifest.webmanifest`, `icon-192.png`, `icon-512.png`.
  Verifica che il nome scelto non sia già un marchio altrui.
- Colori e testi: sono variabili CSS all’inizio di `index.html`.
- Pagine legali sul tuo sito di vendita: privacy policy (spiega che i dati restano sul dispositivo e non li raccogli), termini d’uso, disclaimer “non è consulenza finanziaria, fiscale o legale”.

## Limiti da conoscere
- Nessun account e nessuna sincronizzazione: il passaggio tra dispositivi avviene con il backup in Piano.
- Un file statico si può copiare liberamente: per abbonamenti, licenze o protezione dalla copia serve un servizio con login e pagamenti (backend).
