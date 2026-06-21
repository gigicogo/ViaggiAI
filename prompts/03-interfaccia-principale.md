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

### Struttura della homepage di ViaggiAI

### Com’è fatta la pagina (a parole semplici)

L’app è una pagina unica che cambia contenuto in base a cosa stai facendo. Immaginala come una piccola casa con tre stanze, ma tu vedi sempre solo una stanza alla volta.

#### 🏠 Stanza 1 — La bacheca (schermata iniziale)

È la schermata principale. In alto c’è il titolo dell’app **“ViaggiAI”** e un pulsante ben visibile **“＋ Crea nuovo viaggio”**.  
Sotto, una lista di “cartoline”, una per ogni viaggio salvato: ogni cartolina mostra la destinazione e le date.  
Se non hai ancora creato nessun viaggio, vedi un messaggio di benvenuto che ti invita a crearne uno.

#### ✏️ Stanza 2 — Il modulo di creazione

Quando premi **“Crea nuovo viaggio”**, si apre una schermata con un piccolo modulo:

- destinazione
- data di partenza
- data di ritorno

In fondo ci sono due pulsanti: **“Salva”** e **“Annulla”**.

#### 🔍 Stanza 3 — I dettagli del viaggio

Quando tocchi una cartolina nella bacheca, si apre la schermata dei dettagli:

- in alto un pulsante **“← Torna”** per tornare alla bacheca  
- poi il nome della destinazione e le date  
- e (per ora vuote) le sezioni che riempiremo nelle milestone successive: **budget**, **spese**, **note**.

#### 💾 La memoria nascosta

Ogni volta che crei, modifichi o elimini un viaggio, l’app lo salva automaticamente nella memoria del browser.  
Così, anche se chiudi e riapri, ritrovi tutto.

--- 

## Prompt 2 – Semplificare e ridurre il numero di schermate
> **Prompt**  
>
> Senza stravolgere la struttura né cambiare lo stack (sempre solo HTML, CSS e JavaScript, niente backend), applica questi piccoli miglioramenti di esperienza d’uso:
>
> 1. Quando salvo un nuovo viaggio, mostra un breve messaggio di conferma (ad esempio sopra la lista o sotto il form), che spariscedopo pochi secondi.
> 2. Migliora leggermente lo stato “nessun viaggio”: rendilo più accogliente, con un testo di benvenuto un po’ più caldo ma sempre > sintetico.
> 3. Mantieni separato il codice HTML, CSS e JavaScript come nella versione attuale e aggiungi solo i pezzi necessari per questi miglioramenti, commentando dove hai fatto le modifiche.
>
> Non introdurre ancora budget, spese o note: li aggiungeremo nelle prossime milestone.
> Restituisci il file completo aggiornato.

## Output 2 – Miglioramenti Alla Home page proposta da Qwen (21/06/2026)

## Riepilogo delle modifiche alla homepage

### 1. Toast di conferma

- Aggiunto un elemento `div` con `id="toast"` fuori dal contenitore `.app`, in modo che appaia sopra tutto il resto.
- Definito CSS dedicato con animazione su `opacity` e `translateY` per farlo entrare ed uscire dal basso in modo morbido.
- Creata la funzione `mostraToast(messaggio)` che:
  - imposta il testo del toast
  - lo rende visibile
  - gestisce un timer di 2,5 secondi, resettandolo se vengono salvati più viaggi in rapida successione.
- Chiamata `mostraToast('Viaggio salvato! ✈️')` all’interno di `salvaViaggio`, subito dopo il salvataggio e l’aggiornamento della lista.

### 2. Stato “nessun viaggio” più accogliente

- Resa la sezione vuota più evidente e invitante:
  - sfondo bianco con bordo tratteggiato, per dare l’idea di uno spazio da riempire
  - emoji più grande (🌍)
  - titolo “Benvenuto in ViaggiAI”
  - breve messaggio caldo che invita a creare il primo viaggio.
- Nessun cambiamento alla logica: è solo un miglioramento di testo e aspetto.

### 3. Struttura generale invariata

- Stack e organizzazione restano gli stessi:
  - singolo file HTML che contiene HTML, CSS e JavaScript
  - nessun backend, nessun database esterno
  - dati salvati in `localStorage` come prima.
- Non sono state aggiunte nuove funzionalità di dominio (budget, spese, note): il codice è pronto per affrontare la Milestone 3.

Puoi provare a creare un viaggio: alla conferma vedrai il toast apparire in basso al centro e sparire dopo pochi secondi. Quando questo comportamento ti convince, possiamo passare alla parte di **budget e spese**.





## Note d’uso

- Questo file è il “dietro le quinte” dell’interfaccia: mostra come una serie di prompt ben pensati possono trasformare un’idea vaga in un set di schermate e flussi ragionati.  
- Le risposte dell’AI vengono incollate sotto ogni prompt, così è facile vedere come l’interfaccia evolve nel tempo.  
- Se una versione nuova è migliore, non elimino quella vecchia: la tengo come traccia del percorso.
