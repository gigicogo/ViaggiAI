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

--- 

## Prompt 3 – Schermata di dettaglio del viaggio
> **Prompt**  
>
> Ora concentriamoci sulla schermata di dettaglio di un singolo viaggio.
> 
> Lì voglio vedere:
> – il titolo del viaggio e la destinazione
> – le date
> – il budget totale e il totale speso finora
> – le note e le curiosità
> – la lista delle spese.
> 
> Usando solo HTML, CSS e JavaScript nello stesso stile del codice che abbiamo già, proponimi prima la struttura logica (come se fosse una scheda organizzata in blocchi), poi il modo migliore per implementarla mantenendo la singola pagina che gira nel browser con localStorage per salvare i dati.

## Output 3 – Schermata di dettaglio del viaggio proposta da Qwen (21/06/2026)

## Struttura logica della schermata dettaglio

### 1. Toast di conferma

## Struttura logica della schermata di dettaglio

Immagina la scheda del viaggio come un foglio organizzato in 6 blocchi verticali, dall’alto verso il basso.

### 📍 Blocco 1: Intestazione

In alto:

- pulsante **“← Torna”** per tornare alla bacheca  
- nome della destinazione come titolo grande  
- date del viaggio formattate sotto il titolo  

### 💰 Blocco 2: Riepilogo budget

Una “cartolina” con tre numeri ben visibili:

- **Budget totale** (quanto hai deciso di spendere)  
- **Speso finora** (somma di tutte le spese registrate)  
- **Rimanente** (quanto ti resta; se negativo, indica quanto hai sforato)  

Se il budget non è ancora impostato, compare un messaggio che invita a inserirlo.

### 🧾 Blocco 3: Spese

Una lista di righe, una per ogni spesa registrata. Ogni riga mostra:

- descrizione (es. “Cena ristorante”)  
- importo (es. “€ 45,00”)  
- categoria opzionale (es. “Pasti”, “Trasporti”)  
- un piccolo pulsante **“×”** per eliminare la spesa  

In fondo alla lista:

- pulsante **“＋ Aggiungi spesa”** che apre un piccolo form inline
  - descrizione
  - importo
  - categoria opzionale

### 📝 Blocco 4: Note

- un’area di testo libera dove scrivere appunti, idee, cose da non dimenticare  
- un pulsante **“Salva note”** sotto l’area di testo  

### 💡 Blocco 5: Curiosità

Una lista di elementi testuali (es. “Il museo è chiuso il lunedì”, “Link prenotazione hotel: …”).

Per ogni elemento:

- testo della curiosità  
- pulsante **“×”** per eliminarla  

In fondo alla sezione:

- pulsante **“＋ Aggiungi curiosità”** per creare una nuova voce  

### 🗑️ Blocco 6: Azioni finali

In fondo alla pagina:

- pulsante rosso **“Elimina questo viaggio”** per cancellare l’intero viaggio e tutte le sue informazioni collegate  

## Cosa puoi fare ora con questa schermata

- ✅ Vedere il riepilogo del budget con tre numeri: **budget totale**, **speso**, **rimanente**  
- ✅ Aggiungere spese con descrizione, importo e categoria opzionale  
- ✅ Eliminare singole spese  
- ✅ Scrivere e salvare note libere  
- ✅ Aggiungere ed eliminare curiosità  
- ✅ Modificare il budget in qualsiasi momento  
- ✅ Far sì che tutto si salvi automaticamente in `localStorage`  

Il codice associato è pronto per essere testato.  
Quando questa versione ti convince, il passo successivo sarà la **Milestone 5 (export/import JSON)**.

---

## Prompt 4 – Adattare l'app ale device mobili

> **Prompt**  
>
> Ora voglio ottimizzare ViaggiAI per l’uso su smartphone, senza cambiare lo stack (sempre singola pagina HTML con HTML/CSS/JavaScript e localStorage).
>
>Considera il codice attuale che ti ho fornito e applica SOLO miglioramenti di layout e stile per i dispositivi mobili:
>
> – Assicurati che tutti i testi siano leggibili su schermi piccoli (font size, spaziature, margini).
> – Verifica che i pulsanti principali siano comodamente cliccabili con il pollice (dimensione minima consigliata e spaziatura tra i pulsanti).
> – Evita scroll orizzontali: il contenuto deve adattarsi bene a schermi stretti.
> – Migliora il comportamento delle liste (viaggi, spese, curiosità) su mobile, evitando che gli elementi risultino troppo affollati.
> – Mantieni il “vibe” attuale (colori, stile delle cartoline, toast), solo più ottimizzato per il touch.
>
> Non introdurre nuove funzionalità: lavora solo su CSS e, se necessario, su piccole modifiche HTML.
Mostrami:
> 1) le nuove regole CSS aggiunte o modificate, con un breve commento
> 2) eventuali piccole modifiche HTML (ad esempio classi aggiuntive) strettamente necessarie per il layout mobile.


## Output 4 – Adattamento dell'app per le device mobili proposta da Qwen (21/06/2026)

### Cosa è cambiato per il mobile

### Touch‑friendly

- Tutti i pulsanti hanno `min-height: 48px` (standard Google per touch).
- I pulsanti di eliminazione (`×`) sono più grandi e con sfondo rosso per maggior visibilità.
- Le cartoline hanno un feedback visivo al tocco (`transform: scale(0.98)`).
- `input` e `textarea` hanno `min-height: 48px` e `padding` aumentato.

### Layout responsive

- I pulsanti **“Esporta”** / **“Importa”** si impilano verticalmente su schermi `< 480px`.
- La griglia del budget passa da 3 colonne a 1 colonna su mobile, con layout orizzontale label–valore.
- Il form spese si impila verticalmente su mobile, va a 2 colonne su tablet e a 4 colonne su desktop.
- I pulsanti **“Annulla”** / **“Salva”** si impilano su schermi molto piccoli.

### Ottimizzazioni iOS

- Aggiunto meta tag per web app standalone.
- `font-size: 16px` sugli input per prevenire lo zoom automatico.
- `user-scalable=no` per evitare zoom accidentali.
- `padding` aumentato per compensare la notch.

### Miglioramenti generali

- Focus sugli input con `box-shadow` per un feedback visivo più chiaro.
- Cartoline con `padding` aumentato.
- Toast con `max-width: 90%` per non uscire dallo schermo.
- Pulsante “indietro” con sfondo e dimensioni touch‑friendly.

Ora l’app è completamente usabile da smartphone, tablet e desktop. Provala dal telefono e verifica come cambia l’esperienza di utilizzo.

---

## Note d’uso

- Questo file è il “dietro le quinte” dell’interfaccia: mostra come una serie di prompt ben pensati possono trasformare un’idea vaga in un set di schermate e flussi ragionati.  
- Le risposte dell’AI vengono incollate sotto ogni prompt, così è facile vedere come l’interfaccia evolve nel tempo.  
- Se una versione nuova è migliore, non elimino quella vecchia: la tengo come traccia del percorso.
