# Fase 2 – Milestone del progetto “ViaggiAI”

In questo file raccolgo i prompt che uso per trasformare l’idea dell’app di viaggio in una lista di tappe (milestone) semplici e chiare.

L’obiettivo non è fare subito il piano perfetto, ma creare una prima bozza di percorso che posso poi correggere, semplificare o dettagliare con altri prompt.

---

## Prompt 1 – Creare la prima bozza di piano

Questo è il prompt che uso per chiedere all’AI di propormi una struttura di base del progetto.

>**Prompt**  
>Sto progettando un’app web e mobile come un “taccuino di viaggio intelligente”.  
>L’app serve per raccogliere in un unico posto tutte le idee per i miei viaggi di piacere: destinazioni, percorsi, curiosità, recensioni, budget e costi.  
>
>Voglio lavorare in stile “vibe coding”: io descrivo le intenzioni in italiano semplice e tu mi aiuti a trasformarle in tappe concrete di lavoro.  
> 
>Per favore:  
>1. Proponimi una lista di 6–10 milestone (tappe) per arrivare da “idea grezza” a “prima versione usabile” dell’app.  
>2. Per ogni milestone, dammi:  
>    - un titolo breve  
>    - una descrizione in massimo 3 righe  
>    - cosa devo considerare “fatto” per poterla spuntare.  
> 3. Usa un linguaggio comprensibile anche a chi non è sviluppatore.  
>
> 4. Non scrivere ancora codice: resta a livello di organizzazione del lavoro.
>

## Output 1 – Roadmap proposta da Qwen (18/06/2026)

Ecco una roadmap chiara e pratica per trasformare la tua idea in un'app funzionante, divisa in milestone concrete:

**Milestone 1: Definizione del Viaggio Ideale**
Descrivi su carta o documento le 3-5 funzionalità essenziali che l'app deve avere (es. salvare destinazioni, annotare costi, aggiungere foto).  
**Fatto quando:** Hai una lista prioritaria di massimo 5 funzioni core, con esempi concreti di come le useresti tu.

**Milestone 2: Schizzi delle Schermate Principali**
Disegna a mano o con tool semplici (Figma, Canva) le schermate chiave: home, dettaglio destinazione, aggiunta nota, budget. Non serve perfezione grafica.  
**Fatto quando:** Hai 4-6 schizzi chiari che mostrano cosa vede l'utente in ogni schermata principale.

**Milestone 3: Struttura dei Dati**
Definisci quali informazioni devi salvare per ogni viaggio: nome destinazione, date, costo stimato, note, foto, recensioni linkate.  
**Fatto quando:** Hai un elenco strutturato tipo "ogni viaggio ha: titolo, luogo, data inizio/fine, budget totale, lista spese, galleria foto".

**Milestone 4: Prototipo Navigabile**
Collega gli schizzi tra loro creando un flusso cliccabile (anche solo immagini collegate in Figma o PowerPoint). Deve sembrare un'app vera ma senza logica dietro.  
**Fatto quando:** Puoi "navigare" dall'home alla creazione di un nuovo viaggio e tornare indietro, cliccando sui tuoi schizzi.

**Milestone 5: Scelta degli Strumenti Tecnici**
Decidi se usare strumenti no-code (Bubble, Glide, Adalo) o sviluppare da zero. Considera budget, tempo e competenze.  
**Fatto quando:** Hai scelto la piattaforma/tecnologia e creato un account di prova funzionante.

**Milestone 6: Prima Funzione Costruita**
Implementa UNA sola funzione completa: ad esempio "aggiungere una nuova destinazione con nome e foto". Deve funzionare davvero, salvare i dati e mostrarli.  
**Fatto quando:** Puoi creare un viaggio, salvarlo, vederlo nella lista e aprirlo di nuovo.

**Milestone 7: Gestione Budget Base**
Aggiungi la possibilità di inserire spese per ogni viaggio e vedere il totale speso vs budget previsto.  
**Fatto quando:** Puoi aggiungere almeno 3 spese a un viaggio e vedere il calcolo automatico del totale.

**Milestone 8: Test con Utenti Reali**
Fai provare l'app a 2-3 amici fidati. Chiedi loro di completare un compito specifico (es. "crea un viaggio a Parigi") e osserva dove si bloccano.  
**Fatto quando:** Hai raccolto feedback da almeno 2 persone e identificato 3-5 problemi da risolvere.

**Milestone 9: Rifinitura Essenziale**
Correggi i problemi emersi dai test, migliora testi confusi, aggiusta layout scomodi. Non cercare la perfezione, solo l'usabilità.  
**Fatto quando:** Gli stessi tester riescono a usare l'app senza chiederti spiegazioni.

**Milestone 10: Lancio della Versione Alpha**
Rendi l'app accessibile ad altri oltre ai tester iniziali (condividi link, pubblica su store se mobile, o rendila web-accessibile).  
**Fatto quando:** Almeno 5 persone esterne al tuo circolo ristretto hanno usato l'app e ti hanno dato un feedback.

**Consiglio vibe coding:** Lavora su una milestone alla volta. Quando ne completi una, festeggia! 🎉 Poi passa alla successiva. Non saltare passaggi: ogni tappa costruisce le fondamenta per quella dopo.

---

## Prompt 2 – Sintesi e raggruppamento delle milestone

> **Prompt**  
> Qui sotto trovi la roadmap che mi hai generato per il progetto “ViaggiAI”, con 10 milestone che vanno dall’idea al lancio.  
> 
> Ora voglio una versione più essenziale, utile per guidare davvero lo sviluppo dell’app.  
> 
> Istruzioni operative:  
> 1. Riduci le milestone a **massimo 6**, raggruppando quelle che appartengono alla stessa fase (es. definizione, design, prototipo, sviluppo funzionalità, test, lancio).  
> 2. Per ogni nuova milestone:  
>    - assegna un **titolo breve e descrittivo**, utile da usare anche come nome di branch o etichetta nel project management  
>    - scrivi una **descrizione in 2–3 frasi** focalizzata su cosa deve essere concretamente completato  
>    - definisci un chiaro criterio **“Fatto quando:”** in UNA sola frase verificabile (es.: “posso creare un viaggio, salvarlo e riaprirlo”).  
> 3. Mantieni l’ordine logico di esecuzione: dalla definizione dell’app fino a una prima versione utilizzabile da tester esterni.  
> 4. Restituisci il risultato in elenco numerato (Milestone 1, 2, 3, …).  
> 

## Output 2 – Milestone sintetizzate da Qwen (19/06/2026)

Ecco la roadmap essenziale di ViaggiAI, condensata in 6 milestone operative:

**Milestone 1: Definizione e Architettura**  
Unisci la scelta delle funzionalità core, la struttura dei dati necessari e la selezione degli strumenti tecnici (no-code o sviluppo custom). Questo crea le fondamenta solide su cui costruire senza dover tornare indietro per decisioni strutturali.  
**Fatto quando:** Hai un documento con le 5 funzioni prioritarie, l'elenco dei dati da salvare per ogni viaggio e l'ambiente di sviluppo configurato e pronto all'uso.

**Milestone 2: Design e Flusso Utente**  
Crea gli schizzi delle schermate principali (home, dettaglio, aggiunta nota) e collegali in un prototipo navigabile che simuli l'esperienza reale, anche se solo graficamente. Serve a validare la logica di navigazione prima di scrivere codice.  
**Fatto quando:** Puoi cliccare attraverso gli schizzi per completare un intero flusso, dall'apertura dell'app alla creazione di un nuovo viaggio, senza blocchi logici.

**Milestone 3: Core Funzionante (CRUD)**  
Sviluppa la funzione base di creazione e gestione dei viaggi: l'utente deve poter inserire una destinazione, salvarla nel database, vederla nella lista e riaprirla per modificarla. È il cuore pulsante dell'applicazione.  
**Fatto quando:** Posso creare un nuovo viaggio con titolo e foto, salvarlo, ritrovarlo nella home e aprirlo nuovamente senza errori.

**Milestone 4: Gestione Budget e Spese**  
Implementa la logica finanziaria permettendo di impostare un budget totale e aggiungere singole spese con calcolo automatico del residuo. Questa è la seconda funzionalità distintiva rispetto a una semplice lista di desideri.  
**Fatto quando:** Posso aggiungere almeno 3 spese diverse a un viaggio e vedere il sistema aggiornare automaticamente il totale speso e il budget rimanente.

**Milestone 5: Test e Rifinitura Usabilità**  
Fai provare l'app a 2-3 amici chiedendo loro di eseguire compiti specifici, poi usa i feedback per correggere bug, chiarire testi confusi e migliorare i layout scomodi. L'obiettivo è rendere l'app intuitiva senza bisogno di spiegazioni.  
**Fatto quando:** I tester riescono a creare un viaggio e gestire il budget da soli, senza farmi domande su come procedere.

**Milestone 6: Lancio Alpha Esterno**  
Rendi l'app accessibile pubblicamente (via link web o store) a un gruppo più ampio di utenti esterni al tuo circolo stretto per raccogliere feedback su scala leggermente maggiore. Segna il passaggio da progetto personale a prodotto utilizzabile.  
**Fatto quando:** Almeno 5 persone esterne hanno registrato un account o usato l'app e mi hanno inviato un feedback strutturato.

## Prompt 3 – Tradurre le milestone in lavoro operativo (issue / task)

> **Prompt**  
> Qui sotto trovi la versione sintetica delle 6 milestone operative per il progetto “ViaggiAI”.  
> 
> Ora voglio trasformarle in lavoro concreto da fare, organizzato in attività che posso tracciare in GitHub (issue, task, branch).  
> 
> Istruzioni operative:  
> 1. Per ciascuna delle 6 milestone:  
>    - proponi da 3 a 7 attività concrete (task) necessarie per completarla  
>    - per ogni attività indica:  
>      - un **titolo breve** (usabile come titolo di issue su GitHub)  
>      - una **descrizione operativa** in 2–3 frasi, con cosa va fatto in pratica  
>      - un tipo/area principale (es.: `design`, `frontend`, `backend`, `dati`, `test`, `documentazione`).  
> 2. Per ogni milestone, suggerisci anche un **nome di milestone GitHub** e, se utile, un **prefisso di branch** (es.: `m1-definizione-architettura/`, `m3-core-crud/`).  
> 3. Mantieni l’ordine logico delle milestone (dalla 1 alla 6), così posso usarle come base per creare milestone e issue direttamente nel repository.  
> 4. Restituisci il risultato in formato strutturato, seguendo questo schema:  
>    - Nome milestone  
>    - Nome milestone GitHub suggerito  
>    - Prefisso branch suggerito  
>    - Elenco attività (con titolo, descrizione, tipo).  

## Output 3 – Task operativi generati da Qwen (19/06/2026)

Ecco la scomposizione operativa delle 6 milestone in task tracciabili su GitHub, pronti per essere trasformati in issue.

### Milestone 1: Definizione e Architettura
**Nome milestone GitHub:** `M1-Definizione-Architettura`  
**Prefisso branch:** `m1-def-arch/`

1. **Titolo:** Documentare le 5 funzionalità core prioritarie  
   **Descrizione:** Scrivi un documento (Markdown o Notion) che elenchi le 5 funzioni essenziali con un esempio d'uso concreto per ciascuna. Questo documento servirà come riferimento vincolante per evitare scope creep nelle fasi successive.  
   **Tipo:** Documentazione  

2. **Titolo:** Definire lo schema dati dei viaggi  
   **Descrizione:** Crea un diagramma ER o un file JSON di esempio che specifichi tutti i campi necessari per un viaggio (titolo, date, budget, spese, foto). Assicurati che lo schema supporti tutte le 5 funzionalità core definite nel task precedente.  
   **Tipo:** Dati / Backend  

3. **Titolo:** Selezionare e configurare lo stack tecnologico  
   **Descrizione:** Scegli la piattaforma (no-code o framework custom) basandoti su budget e competenze, e crea un repository/progetto di prova funzionante. Documenta la scelta e i motivi nel README del progetto principale.  
   **Tipo:** Infrastruttura / Setup  

4. **Titolo:** Configurare ambiente di sviluppo locale  
   **Descrizione:** Installa tutte le dipendenze necessarie, configura linter/formatter e verifica che il progetto giri localmente senza errori. Aggiungi un file `.env.example` e istruzioni di setup nel README per garantire riproducibilità.  
   **Tipo:** Infrastruttura / DevOps  

---

### Milestone 2: Design e Flusso Utente
**Nome milestone GitHub:** `M2-Design-Flusso`  
**Prefisso branch:** `m2-design/`

1. **Titolo:** Creare wireframe schermate principali  
   **Descrizione:** Disegna le 4-6 schermate chiave (home, dettaglio viaggio, form creazione, gestione budget) usando Figma, Excalidraw o carta. Concentrati sulla gerarchia delle informazioni, non sull'estetica finale.  
   **Tipo:** Design / UX  

2. **Titolo:** Collegare wireframe in prototipo navigabile  
   **Descrizione:** Crea un flusso cliccabile che permetta di navigare dall'home alla creazione di un viaggio e ritorno, simulando l'esperienza reale. Usa lo strumento di prototipazione del tuo tool di design o collega immagini in un PDF interattivo.  
   **Tipo:** Design / Prototipazione  

3. **Titolo:** Validare flusso con walkthrough interno  
   **Descrizione:** Esegui tu stesso il flusso completo nel prototipo verificando che non ci siano vicoli ciechi o passaggi illogici. Documenta eventuali incongruenze emerse e correggi gli schizzi prima di passare allo sviluppo.  
   **Tipo:** Design / QA  

---

### Milestone 3: Core Funzionante (CRUD)
**Nome milestone GitHub:** `M3-Core-CRUD`  
**Prefisso branch:** `m3-core-crud/`

1. **Titolo:** Implementare modello/database Viaggio  
   **Descrizione:** Crea la tabella/collection "Viaggi" nello stack scelto, mappando tutti i campi definiti nella M1. Verifica che sia possibile inserire e recuperare un record via API o query diretta.  
   **Tipo:** Backend / Dati  

2. **Titolo:** Creare form di inserimento nuovo viaggio  
   **Descrizione:** Sviluppa la schermata frontend con campi titolo, destinazione, date e upload foto, collegandola al salvataggio nel database. Gestisci validazione base dei campi obbligatori e feedback visivo di successo/errore.  
   **Tipo:** Frontend  

3. **Titolo:** Implementare lista viaggi nella home  
   **Descrizione:** Crea la schermata home che recupera e mostra tutti i viaggi salvati in ordine cronologico inverso. Ogni elemento della lista deve essere cliccabile e portare alla schermata di dettaglio.  
   **Tipo:** Frontend  

4. **Titolo:** Creare schermata dettaglio/modifica viaggio  
   **Descrizione:** Sviluppa la vista che mostra tutti i dati di un singolo viaggio e permette la modifica di ogni campo. Le modifiche devono persistere nel database e riflettersi immediatamente nella lista home.  
   **Tipo:** Frontend / Backend  

5. **Titolo:** Test end-to-end flusso CRUD completo  
   **Descrizione:** Verifica manualmente che sia possibile creare un viaggio, vederlo nella lista, aprirlo, modificarlo e salvare senza errori. Documenta il test con screenshot o breve video come prova di completamento.  
   **Tipo:** Test / QA  

---

### Milestone 4: Gestione Budget e Spese
**Nome milestone GitHub:** `M4-Budget-Spese`  
**Prefisso branch:** `m4-budget/`

1. **Titolo:** Estendere schema dati con entità Spesa  
   **Descrizione:** Aggiungi la relazione uno-a-molti tra Viaggio e Spesa (importo, descrizione, data, categoria). Aggiorna il modello Viaggio per includere il campo budget totale predefinito.  
   **Tipo:** Dati / Backend  

2. **Titolo:** Implementare form aggiunta spesa  
   **Descrizione:** Crea un componente UI per aggiungere una nuova spesa all'interno del dettaglio viaggio, con validazione numerica dell'importo. Dopo il salvataggio, la lista spese deve aggiornarsi senza ricaricare la pagina.  
   **Tipo:** Frontend  

3. **Titolo:** Calcolare e mostrare totale speso e residuo  
   **Descrizione:** Implementa la logica (frontend o backend) che somma tutte le spese di un viaggio e sottrae dal budget totale. Mostra entrambi i valori in modo prominente nel dettaglio viaggio, evidenziando visivamente se il budget è superato.  
   **Tipo:** Frontend / Logica Business  

4. **Titolo:** Test scenario budget con multiple spese  
   **Descrizione:** Aggiungi almeno 3 spese diverse a un viaggio e verifica che il calcolo sia corretto e si aggiorni ad ogni aggiunta/modifica/cancellazione. Testa anche il caso limite di budget esaurito e superato.  
   **Tipo:** Test / QA  

---

### Milestone 5: Test e Rifinitura Usabilità
**Nome milestone GitHub:** `M5-Test-Rifinitura`  
**Prefisso branch:** `m5-test-usability/`

1. **Titolo:** Preparare script di test per utenti esterni  
   **Descrizione:** Scrivi 3-5 compiti specifici da far eseguire ai tester (es. "Crea un viaggio a Lisbona con budget 800€ e aggiungi 2 spese"). Includi un semplice form o template per raccogliere feedback strutturato.  
   **Tipo:** Test / Documentazione  

2. **Titolo:** Condurre sessioni di test con 2-3 amici  
   **Descrizione:** Osserva i tester mentre eseguono i compiti senza intervenire, annotando dove esitano, sbagliano o chiedono chiarimenti. Registra le sessioni (con permesso) o prendi note dettagliate in tempo reale.  
   **Tipo:** Test / UX Research  

3. **Titolo:** Triaging e prioritizzazione feedback  
   **Descrizione:** Raccogli tutti i problemi emersi e categorizzali in bug critici, problemi di usabilità e miglioramenti nice-to-have. Crea issue GitHub separate per ciascuno, assegnando priorità ai blocchi funzionali.  
   **Tipo:** Project Management / QA  

4. **Titolo:** Correggere bug e migliorare testi/layout  
   **Descrizione:** Risolvi le issue prioritarie emerse dai test, focalizzandoti su chiarezza dei messaggi, etichette dei bottoni e flussi confusi. Non introdurre nuove funzionalità: l'obiettivo è solo rendere l'esistente intuitivo.  
   **Tipo:** Frontend / Fix  

5. **Titolo:** Verifica usabilità post-fix con stessi tester  
   **Descrizione:** Fai rieseguire gli stessi compiti agli stessi tester per confermare che i problemi siano risolti e non ne siano emersi di nuovi. La milestone si chiude solo quando completano il flusso senza domande.  
   **Tipo:** Test / Validazione  

---

### Milestone 6: Lancio Alpha Esterno
**Nome milestone GitHub:** `M6-Lancio-Alpha`  
**Prefisso branch:** `m6-alpha-launch/`

1. **Titolo:** Configurare deployment produzione/staging  
   **Descrizione:** Prepara l'ambiente pubblico (hosting web, build mobile o link condivisibile) separato dall'ambiente di sviluppo. Verifica che tutti i dati e le funzionalità funzionino identicamente all'ambiente locale.  
   **Tipo:** DevOps / Infrastruttura  

2. **Titolo:** Creare onboarding e canale feedback per alpha tester  
   **Descrizione:** Prepara un messaggio/email di benvenuto con link all'app, istruzioni minime e canale dedicato per inviare feedback (form, email, Discord). Riduci al minimo l'attrito iniziale per massimizzare la partecipazione.  
   **Tipo:** Comunicazione / Product  

3. **Titolo:** Invitare 5+ utenti esterni e monitorare utilizzo  
   **Descrizione:** Condividi l'app con persone fuori dal tuo circolo stretto e traccia quante completano la registrazione o il primo viaggio. Raccogli attivamente feedback entro 7 giorni dall'invito.  
   **Tipo:** Launch / Analytics  

4. **Titolo:** Documentare risultati alpha e next steps  
   **Descrizione:** Sintetizza in un documento interno i feedback ricevuti, le metriche di utilizzo e le lezioni apprese. Definisci le priorità per la prossima iterazione basandoti sui dati reali, non sulle ipotesi.  
   **Tipo:** Documentazione / Planning  

> Nota pratica per il vibe coding: non creare tutte le issue subito. Apri quelle della Milestone 1 ora, e crea le successive solo quando la milestone corrente è al 70–80% completata. Questo mantiene il backlog pulito e ti permette di adattare i task in base a ciò che impari strada facendo.

---

## Note d’uso

- Questo file non è pensato per essere “perfetto”: è il diario di come il piano del progetto evolve mentre dialogo con l’AI.  
- Ogni volta che ottengo una versione migliore della lista di milestone, posso aggiungerla qui sotto con la data, invece di cancellare la precedente.  
- Ciò consente di vedere non solo il risultato finale, ma anche i passaggi intermedi.
