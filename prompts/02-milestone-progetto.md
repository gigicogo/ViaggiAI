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

## Prompt 2 – Semplificare e rinominare le milestone

Una volta ottenuta la prima proposta, voglio rendere il piano ancora più leggibile per un pubblico non tecnico.

> **Prompt**  
> Ecco la lista di milestone che mi hai proposto (incollo sotto la tua risposta).  
> 
> Ti chiedo di semplificarla:  
> 1. Riduci le milestone a un massimo di 6, raggruppando quelle troppo simili.  
> 2. Rinomina ogni milestone con un titolo molto chiaro, come se dovesse essere compreso da un lettore curioso ma non tecnico.  
> 3. Per ogni milestone, mantieni:  
>    - un titolo breve  
>    - una descrizione in massimo 2 righe  
>    - cosa consideriamo “fatto” in una sola frase.  
> 4. Restituisci il risultato in forma di elenco numerato.

Anche qui, sotto il prompt incollerò la nuova versione della lista di milestone.

---

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
