# Fase 3 – Interfaccia principale dell’app “ViaggiAI”

In questo file raccolgo i prompt che uso per farmi aiutare dall’AI a immaginare le schermate principali dell’app: cosa si vede, cosa si può fare, come ci si muove da una parte all’altra.

L’obiettivo è avere una struttura chiara dell’esperienza utente prima ancora di pensare ai dettagli grafici o al codice.

---

## Prompt 1 – Disegnare le schermate principali

Questo è il prompt che uso per chiedere all’AI una prima proposta di struttura dell’interfaccia.

> **Prompt**  
> Usando il contesto di ViaggiAI che ti ho descritto nelle Istruzioni del progetto, aiutami a progettare la homepage dell’app.
>
> Voglio:
> – vedere la lista dei viaggi salvati (titolo, destinazione, date)
> – avere un pulsante chiaro “Crea nuovo viaggio”
> – poter aprire un viaggio per vedere i dettagli.
>
> Descrivimi prima in parole semplici com’è strutturata la pagina (sezioni, elementi principali) e solo dopo proponimi il codice o > i componenti necessari, usando solo HTML, CSS e JavaScript.


## Output 1 – Struttura della Home page proposta da Qwen (18/06/2026)

Struttura della Homepage di ViaggiAI
Com'è fatta la pagina (a parole semplici)
L'app è una pagina unica che cambia contenuto in base a cosa stai facendo. Immaginala come una piccola casa con tre stanze, ma tu vedi sempre solo una stanza alla volta:
🏠 Stanza 1 — La Bacheca (quella che vedi all'apertura)
È la schermata principale. In alto c'è il titolo dell'app "ViaggiAI" e un pulsante ben visibile "＋ Crea nuovo viaggio". Sotto, una lista di cartoline, una per ogni viaggio salvato: ogni cartolina mostra la destinazione e le date. Se non hai ancora creato nessun viaggio, vedi un messaggio di benvenuto che ti invita a crearne uno.
✏️ Stanza 2 — Il Modulo di Creazione
Quando premi "Crea nuovo viaggio", si apre una schermata con un piccolo modulo: destinazione, data di partenza, data di ritorno. Due pulsanti in fondo: Salva e Annulla.
🔍 Stanza 3 — I Dettagli del Viaggio
Quando tocchi una cartolina nella bacheca, si apre la schermata dei dettagli: in alto un pulsante "← Torna" per tornare alla bacheca, poi il nome della destinazione, le date, e (per ora vuote) le sezioni che riempiremo nelle milestone successive: budget, spese, note.
💾 La memoria nascosta
Ogni volta che crei, modifichi o elimini un viaggio, l'app lo salva automaticamente nella memoria del browser. Così, anche se chiudi e riapri, ritrovi tutto.

---

## Prompt 2 – Semplificare e ridurre il numero di schermate

La prima proposta dell’AI può essere troppo complessa. Con questo prompt chiedo una versione più semplice, adatta a una prima versione dell’app.

> **Prompt**  
> Ecco le schermate principali che mi hai proposto (incollo sotto la tua risposta).  
> 
> Ti chiedo di semplificarle:  
> 1. Riduci il numero di schermate al minimo indispensabile per avere una prima versione utilizzabile dell’app (massimo 5 schermate).  
> 2. Raggruppa le funzioni simili nella stessa schermata, quando ha senso farlo.  
> 3. Per ogni schermata, riscrivi la descrizione in massimo 3 righe, mettendo in evidenza:  
>    - lo scopo della schermata  
>    - le azioni principali  
>    - il tipo di informazione che l’utente trova.  
> 4. Restituisci il risultato in forma di elenco numerato.

Anche in questo caso, sotto il prompt incollerò la nuova versione della lista di schermate.

---

## Prompt 3 – Collegare schermate e flussi (navigazione)

Una volta definite le schermate principali, voglio chiarire come ci si muove da una all’altra (i “percorsi” dell’utente).

> **Prompt**  
> Abbiamo definito l’elenco delle schermate principali per l’app “ViaggiAI”.  
> Ora ti chiedo di concentrarti sulla navigazione:  
> 1. Disegna, in forma testuale, i principali flussi dell’utente, ad esempio:  
>    - “da zero a primo viaggio creato”  
>    - “aggiornare il budget di un viaggio”  
>    - “rileggere le note e le curiosità di un viaggio passato”.  
> 2. Per ogni flusso, descrivi passo per passo quali schermate vengono toccate e che azioni compie l’utente.  
> 3. Restituisci il tutto in formato elenco puntato, uno per flusso, con i passi numerati.  
> 4. Mantieni un linguaggio semplice e visuale, come se stessi raccontando la scena a voce.

Sotto questo prompt incollerò la risposta dell’AI, che rappresenta la prima versione dei flussi dell’app.

---

## Prompt 4 – Suggerimenti per la resa visiva

Infine, voglio farmi aiutare dall’AI a dare qualche indicazione di stile, per rendere l’interfaccia coerente con la “vibe” dell’app.

> **Prompt**  
> Considerando l’idea di “taccuino di viaggio intelligente” e le schermate che abbiamo definito, ti chiedo di:  
> 1. Suggerire uno stile visivo generale per l’app (colori, tono, livello di semplicità).  
> 2. Dare per ogni schermata 2–3 indicazioni pratiche (es.: “usa una grande call-to-action”, “mostra le date in alto”, “metti le note in una colonna laterale”).  
> 3. Restare su indicazioni di design comprensibili anche a chi non è designer (evita termini troppo tecnici).  
> 4. Restituire il risultato in elenco strutturato per schermata.

Queste indicazioni non sostituiscono il lavoro di un designer, ma aiutano a mantenere una certa coerenza tra l’idea iniziale, i flussi e l’aspetto dell’app.

---

## Note d’uso

- Questo file è il “dietro le quinte” dell’interfaccia: mostra come una serie di prompt ben pensati possono trasformare un’idea vaga in un set di schermate e flussi ragionati.  
- Le risposte dell’AI vengono incollate sotto ogni prompt, così è facile vedere come l’interfaccia evolve nel tempo.  
- Se una versione nuova è migliore, non elimino quella vecchia: la tengo come traccia del percorso.
