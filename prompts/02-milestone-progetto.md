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

Vuoi che approfondiamo insieme la prima milestone per definire meglio le funzionalità core?

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
> Sotto questo prompt incollerò la roadmap originale a 10 milestone: usala come base per la sintesi, senza aggiungere nuove idee non presenti lì.

---

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

## Prompt 3 – Collegare le milestone all’articolo e al repository

Infine, voglio che le milestone siano collegate sia all’articolo che al laboratorio su GitHub.

> **Prompt**  
> Abbiamo definito la lista finale di milestone per il progetto “ViaggiAI”.  
> Ora ti chiedo di:  
> 1. Per ogni milestone, suggerire in una riga che tipo di contenuto potrei mostrare:  
>    - nell’articolo (es.: spiegazione, screenshot, mini storia, ecc.)  
>    - nel repository GitHub (es.: file di prompt, cartella con screenshot, demo, ecc.).  
> 2. Restituire il tutto in formato tabella Markdown con queste colonne:  
>    - Milestone  
>    - Cosa racconto nell’articolo  
>    - Cosa salvo nel repository.  
> 3. Usa un linguaggio semplice e concreto.

Questa tabella sarà la base per collegare in modo chiaro testo dell’articolo, prompt e file del repository.

---

## Note d’uso

- Questo file non è pensato per essere “perfetto”: è il diario di come il piano del progetto evolve mentre dialogo con l’AI.  
- Ogni volta che ottengo una versione migliore della lista di milestone, posso aggiungerla qui sotto con la data, invece di cancellare la precedente.  
- Il lettore potrà così vedere non solo il risultato finale, ma anche i passaggi intermedi.
