# Rubrica Clienti – per ottico/oculista

App web gratuita, senza server e senza account, per tenere la rubrica dei clienti.
Ogni cliente ha uno **storico di visite**. Per ogni visita si registrano:

- date (visita, prescrizione, prossimo controllo)
- gradazione per **lontano** (sempre visibile) e, se servono, per **vicino** e **media distanza**:
  sfera, cilindro, asse, add., prisma, base, visus per ogni occhio; schema TABO
- distanza interpupillare, lenti a contatto (riquadri chiudibili)
- tipo di lente per occhio, montatura, prezzo, note

Del cliente si salvano nome, cognome, telefono, data di nascita, codice fiscale, indirizzo, e-mail,
anamnesi e note generali.

- Un solo file `index.html`: si apre in qualsiasi browser.
- I dati restano **nel browser del computer** dove viene usata (nessun invio a internet).
- Pulsanti grandi, testo grande, tutto in italiano.
- Tre schermate: **lista clienti** → **scheda cliente** (anagrafica + storico visite) → **visita**.
- I dati usati di rado stanno in riquadri chiudibili ("▶ Gradazione per vicino", "▶ Lenti a contatto"...)
  che si aprono con un click e si aprono da soli quando contengono dati.
- "Copia i valori dall'ultima visita" per compilare velocemente una nuova visita.
- **Copia di sicurezza**: scarica un file `.json` con tutta la rubrica. **Ripristina**: lo ricarica.
- Funziona anche senza connessione dopo la prima apertura (si può "installare" sul desktop/telefono).
- Stampa della scheda cliente.

## Pubblicare gratis su GitHub Pages

1. Crea un repository su GitHub (es. `rubrica-clienti`) e carica questi file:
   `index.html`, `manifest.json`, `sw.js`, `icona.svg`.
2. Nel repository: **Settings → Pages → Build and deployment → Source: "Deploy from a branch"**,
   Branch `main`, cartella `/ (root)` → **Save**.
3. Dopo 1-2 minuti l'app è online su `https://TUO-UTENTE.github.io/rubrica-clienti/`.
4. Sul computer dell'oculista: apri quel link e **aggiungilo ai preferiti / crea un collegamento sul desktop**
   (in Chrome: menu ⋮ → "Installa app" oppure "Salva e condividi → Crea scollegamento").

## Importante da sapere

- I dati sono salvati nel browser di **quel** computer. Se si cambia computer o browser, o si
  cancellano i dati di navigazione, la rubrica va ripristinata da una copia di sicurezza.
- Consiglio: premere "Salva copia di sicurezza" una volta a settimana e tenere il file in una cartella
  o inviarselo per email.
