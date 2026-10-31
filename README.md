# Scelta in gioco

Laboratorio interattivo di orientamento per le terze medie: **110 professioni**, nove criteri di scelta, due fasi e una scaletta di 120 minuti. Progetto di Fausto Sana.

Il sito è autonomo: HTML, CSS e JavaScript, senza ChatGPT, API, chiavi, server applicativo, account o dipendenze da installare. Questo repository contiene il codice; il caricamento dei file non attiva da solo la pubblicazione.

## Pubblicare su GitHub Pages

Quando vuoi rendere il gioco accessibile pubblicamente:

1. Apri **Settings → Pages** di questo repository.
2. In **Build and deployment**, seleziona **Deploy from a branch**.
3. Scegli il branch **main** e la cartella **/ (root)**.
4. Premi **Save** e attendi il completamento della pubblicazione. GitHub mostrerà il link effettivo e il pulsante **Visit site**.

L’indirizzo previsto dopo l’attivazione è `https://sanafausto-byte.github.io/sceltaingioco/`. Non è un link confermato finché GitHub Pages non termina il deployment. Gli aggiornamenti successivi ai file di main saranno pubblicati automaticamente.

**Visibilità:** il repository è pubblico. GitHub Pages, con questa configurazione, rende il gioco pubblico e senza password. Se desideri un sito riservato, non attivare Pages: usa un hosting con un vero controllo di accesso. Un codice scritto nel JavaScript non protegge i contenuti.

## Altri hosting

Puoi caricare `index.html`, `style.css`, `data.js`, `app.js` e `.nojekyll` su qualsiasi hosting statico, nella stessa cartella. Non occorre una compilazione. I collegamenti relativi funzionano anche quando il sito si trova in una sottocartella.

## Provarlo sul computer

Scarica il repository con **Code → Download ZIP**, estrai i file e apri `index.html`. Per un’origine locale stabile e un salvataggio più prevedibile, se hai Python installato, dalla cartella esegui:

```bash
python -m http.server 8000
```

Poi apri `http://localhost:8000`. Il server serve soltanto i file e non raccoglie risposte.

## Come condurre il laboratorio

Apri **Guida orientatore** nel sito per la scaletta completa.

- **Preparazione, 00–25:** gruppi da 4–5, presentazione della bussola dei nove criteri e regole.
- **Fase 1, 25–55:** ogni studente sceglie una professione, assegna 5 fiches su almeno 3 colori e motiva almeno 3 criteri. Massimo 2 fiches sullo stesso criterio. Cerca nel catalogo per nome o parola chiave.
- **Passaggio, 55–60:** salva le schede personali.
- **Fase 2, 60–112:** confrontate i percorsi A/B di uno scenario con 7 fiches su almeno 5 criteri; motivatele, pescate un imprevisto e rivedete l’ipotesi. Spostate almeno 2 fiches oppure motivate perché le confermate. Concludete con un pitch.
- **Sintesi, 112–120:** osservate i criteri emersi e completate l’exit ticket con 3 criteri personali, un dubbio e un’azione entro due settimane.

Una sessione ospita fino a 6 schede personali: è pensata per un tavolo. Con la LIM puoi usare schede esemplificative e far compilare agli altri studenti le risposte su carta. Il gioco non assegna automaticamente una scuola o una professione.

## Risposte e privacy

Le risposte sono salvate nel browser del singolo dispositivo tramite `localStorage`, quando disponibile. Non esiste sincronizzazione tra telefoni, raccolta centrale delle risposte o classifica in tempo reale. Non ci sono analytics né font esterni nel codice fornito. Il provider di hosting può gestire i propri log di accesso.

Usa soprannomi ed evita informazioni personali sensibili. Su un dispositivo condiviso, scarica prima la sintesi e poi usa **Nuova partita** per cancellare la sessione. Il browser o la navigazione privata potrebbero eliminare i dati: esporta sempre ciò che vuoi conservare.

**Scarica la sintesi** esporta un file di testo; **Stampa / Salva PDF** apre la stampa del browser. Passando dal dominio ChatGPT a questo sito le vecchie risposte non si trasferiscono, perché appartengono all’origine del browser precedente.

## File da modificare

| File | Contenuto |
| --- | --- |
| `data.js` | Professioni, nove criteri, scenari, imprevisti e scaletta |
| `app.js` | Regole, ricerca, schede, salvataggio e sintesi |
| `style.css` | Aspetto e adattamento a desktop e smartphone |
| `index.html` | Struttura, guida orientatore e contatti |
| `.nojekyll` | Pubblicazione dei file statici senza Jekyll |

Le professioni sono indicizzate: aggiungi nuove carte in coda se vuoi mantenere compatibili le sessioni già salvate.

## Fonte e contatti

Adattamento didattico dai [nove criteri per la scelta della scuola secondaria di II grado di Fausto Sana, Magazine ASNOR](https://magazine.asnor.it/9-criteri-per-la-scelta-della-scuola-secondaria-di-ii-grado/). Le professioni sono spunti di esplorazione; requisiti di accesso alle professioni e offerta formativa vanno verificati presso fonti ufficiali.

[faustosana.it](https://www.faustosana.it) · [info@faustosana.it](mailto:info@faustosana.it) · [LinkedIn](https://www.linkedin.com/in/fausto-sana/)
