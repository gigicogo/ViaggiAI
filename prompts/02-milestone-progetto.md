# Fase 2 – Milestone del progetto “ViaggiAI”

In questo file raccolgo i prompt che uso per trasformare l’idea dell’app di viaggio in una lista di tappe (milestone) semplici e chiare.

L’obiettivo non è fare subito il piano perfetto, ma creare una prima bozza di percorso che posso poi correggere, semplificare o dettagliare con altri prompt.

---

## Prompt 1 – Creare la prima bozza di piano

Questo è il prompt che uso per chiedere all’AI di propormi una struttura di base del progetto.

> **Prompt**  
> Proponimi una lista di 5–6 milestone (tappe) per arrivare da “idea grezza” a “prima versione usabile” di questa app per organizzare i viaggi.
> 
> Per ogni milestone dammi:
>    - un titolo breve
>    - una breve descrizione
>    - cosa devo considerare “fatto” per poterla spuntare.
>

## Output 1 – Roadmap proposta da Qwen (18/06/2026)

Ecco una proposta di 6 milestone per costruire **ViaggiAI** passo dopo passo, rispettando un approccio conservativo e la preferenza per HTML/JS puro con `localStorage`.

### Milestone 1: Lo "Scheletro" (Struttura base)

- **Descrizione:** Creiamo un unico file `index.html` con una struttura pulita. Implementiamo la logica base per creare un nuovo viaggio (nome destinazione, date inizio/fine) e salvarlo in memoria temporanea.
- **Cosa è "fatto":**
  - Hai un form minimale che accetta destinazione e date.
  - Cliccando "Salva", il viaggio appare in una lista sotto il form.
  - L'interfaccia è leggibile sia su PC che su mobile (viewport impostato correttamente).

### Milestone 2: La persistenza (niente più perdite)

- **Descrizione:** Risolviamo subito il problema che avevi nell'app di finanze: i dati devono sopravvivere al refresh della pagina. Usiamo `localStorage` per salvare l'array dei viaggi.
- **Cosa è "fatto":**
  - Se chiudi e riapri il browser, i viaggi creati sono ancora lì.
  - Ogni viaggio nella lista ha un pulsante "Elimina" per gestire gli errori.

### Milestone 3: Il cuore finanziario (budget e spese)

- **Descrizione:** Entriamo nel dettaglio di ogni viaggio. Aggiungiamo la possibilità di impostare un **budget totale** e di registrare singole spese (importo, descrizione, categoria opzionale).
- **Cosa è "fatto":**
  - Puoi cliccare su un viaggio esistente per aprirne i dettagli.
  - All'interno dei dettagli puoi aggiungere spese e vedere un contatore "Speso vs Budget".

### Milestone 4: Il taccuino (note e curiosità)

- **Descrizione:** Trasformiamo l'app da semplice foglio di calcolo a taccuino. Aggiungiamo un'area di testo libera per note generali e una sezione per "Curiosità" o link utili (ad esempio il link alla prenotazione hotel).
- **Cosa è "fatto":**
  - Ogni viaggio ha una sua sezione "Note" salvabile.
  - L'interfaccia permette di scorrere facilmente tra budget e note.

### Milestone 5: Backup e portabilità (file JSON)

- **Descrizione:** Come per la tua app di finanze, implementiamo export/import. Questo ti permette di fare backup manuali o spostare i dati tra dispositivi senza dipendere solo dal browser.
- **Cosa è "fatto":**
  - Un pulsante "Esporta viaggi" scarica un file `.json`.
  - Un pulsante "Importa viaggi" carica il file e aggiorna la lista.

### Milestone 6: Rifinitura "vibe" (UX mobile)

- **Descrizione:** Rendiamo l'esperienza fluida. Miglioriamo i pulsanti per il touch, aggiungiamo feedback visivi quando si salva e ci assicuriamo che non ci siano scroll orizzontali accidentali su schermi piccoli.
- **Cosa è "fatto":**
  - L'app sembra una "web app" nativa sul telefono.
  - I colori e i font sono coerenti e rilassanti (stile "vibe coding").

**Domanda di chiarimento prima di iniziare la milestone 1:**  
Preferisci che l'app mostri subito la lista dei viaggi passati (come una dashboard) o che parta direttamente dalla schermata di creazione di un nuovo viaggio?

---

## Prompt 2 – Sintesi e raggruppamento delle milestone

> **Prompt**  
> Le milestone che mi hai proposto vanno bene per me, ma sono troppo tecniche.
>
> Riscrivimi le STESSE 6 milestone:
>    - usando un linguaggio comprensibile a chi non sa cosa sono HTML, JavaScript, localStorage o file JSON
>    - senza nominare file, tecnologie o termini tecnici
>    - parlando solo di cosa l’utente può fare in ogni fase (es. “posso creare un viaggio”, “posso aggiungere spese”, “posso fare un backup dei miei viaggi”)
>    - mantenendo per ogni milestone:
>    - un titolo breve
>    - 2–3 frasi di descrizione
>    - una frase che inizia con “Fatto quando:” che spiega in modo concreto cosa devo essere in grado di fare.
>
> Non aggiungere nuove milestone, limita a riscrivere queste 6 in modo più semplice.
> 

## Output 2 – Milestone sintetizzate da Qwen (21/06/2026)

Ecco le 6 milestone riscritte in linguaggio semplice:

### Milestone 1: Creare il primo viaggio

- **Descrizione:** L'app permette di inserire le informazioni base di un viaggio: dove vai e quando. Una volta salvato, il viaggio appare in una lista che puoi consultare.
- **Fatto quando:** Posso scrivere destinazione e date, cliccare un pulsante, e vedere il mio viaggio comparire nella lista.

### Milestone 2: L'app si ricorda tutto

- **Descrizione:** I viaggi che creo non spariscono quando chiudo l'app o il browser. Rimangono salvati e posso ritrovarli ogni volta che apro l'app, anche dopo giorni. Posso anche eliminare un viaggio se ho sbagliato.
- **Fatto quando:** Chiudo e riapro l'app, e tutti i miei viaggi sono ancora lì, pronti da consultare.

### Milestone 3: Tenere traccia delle spese

- **Descrizione:** Per ogni viaggio posso impostare un budget totale e registrare tutte le spese che faccio, una per una. L'app mi mostra quanto ho già speso rispetto al budget che mi sono dato.
- **Fatto quando:** Posso aprire un viaggio, vedere quanto ho speso e aggiungere nuove spese con descrizione e importo.

### Milestone 4: Aggiungere note e dettagli

- **Descrizione:** Oltre ai soldi, posso scrivere appunti liberi per ogni viaggio: idee, cose da non dimenticare, link utili per prenotazioni o informazioni interessanti che trovo durante la preparazione.
- **Fatto quando:** Posso scrivere e salvare note personali per ogni viaggio, oltre a gestire il budget.

### Milestone 5: Fare backup dei dati

- **Descrizione:** Posso scaricare una copia di tutti i miei viaggi in un unico file, così ho un backup di sicurezza. Se cambio dispositivo o cancello i dati per sbaglio, posso ricaricare tutto da quel file.
- **Fatto quando:** Posso esportare tutti i miei viaggi in un file e, se serve, reimportarli per recuperarli.

### Milestone 6: Usare l'app dal telefono

- **Descrizione:** L'app diventa comoda da usare anche sullo smartphone, con pulsanti grandi e un'interfaccia che si adatta bene allo schermo piccolo. L'esperienza è fluida e piacevole, come un'app nativa.
- **Fatto quando:** Posso usare l'app dal telefono senza problemi, con pulsanti facili da toccare e niente elementi che si sovrappongono o escono dallo schermo.

---

Nota pratica per il vibe coding: non creare tutte le issue subito. Apri quelle della Milestone 1 ora, e crea le successive solo quando la milestone corrente è al 70–80% completata. Questo mantiene il backlog pulito e ti permette di adattare i task in base a ciò che impari strada facendo.
   
---

## Note d’uso

- Questo file non è pensato per essere “perfetto”: è il diario di come il piano del progetto evolve mentre dialogo con l’AI.  
- Ogni volta che ottengo una versione migliore della lista di milestone, posso aggiungerla qui sotto con la data, invece di cancellare la precedente.  
- Ciò consente di vedere non solo il risultato finale, ma anche i passaggi intermedi.
