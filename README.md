# Angular Material Scientific Calculator

Applicazione calcolatrice interattiva sviluppata con **Angular (v17+)**, focalizzata sull'integrazione della libreria UI **Angular Material** e sulla gestione della logica di calcolo dinamica.

## Descrizione
Il progetto implementa una calcolatrice funzionale ospitata all'interno di un componente dedicato (`TableComponent`). L'interfaccia utente è costruita utilizzando i componenti avanzati di Google (Material Design), garantendo un look professionale e reattivo. La logica di calcolo sfrutta il parsing dinamico delle stringhe per eseguire operazioni aritmetiche in tempo reale.



## Funzionamento del Sistema:
* **Integrazione Angular Material**: Utilizzo di moduli specifici come `MatButtonModule`, `MatFormFieldModule` e `MatInputModule` per un'esperienza utente moderna e accessibile.
* **Componentizzazione**: Suddivisione dell'app in un componente principale (`AppComponent`) che funge da layout e un componente specializzato (`TableComponent`) per la logica di business.
* **String Buffering Logic**: Accumulo degli input dell'utente in una variabile di tipo stringa attraverso la funzione `clickButton()`, simulando il comportamento di una calcolatrice reale.
* **Dynamic Expression Evaluation**: Utilizzo della funzione `eval()` per processare la stringa di input come espressione matematica e restituire il risultato immediato.
* **Layout Management**: Organizzazione dei tasti tramite una struttura tabellare CSS-styled per garantire l'allineamento perfetto dei tasti numerici e degli operatori.
* **Async Animations**: Configurazione di `provideAnimationsAsync()` nell'app config per supportare i feedback visivi (ripple effect) tipici del Material Design.

## Tecnologie e Concetti
* **Angular Material**: Libreria di componenti UI basata su Material Design.
* **Event Handling**: Gestione dei click sui tasti per aggiornare lo stato dell'input o resettare la memoria (`cancel`).
* **Standalone Components**: Architettura priva di moduli (NgModules) per una gestione più snella delle dipendenze.
* **CSS Flexbox & Centering**: Tecniche di posizionamento avanzate per centrare l'applicazione nella viewport del browser.

## Struttura dell'Interfaccia
| Categoria | Componenti Material | Scopo |
| :--- | :--- | :--- |
| **Display** | `matInput` (Disabled) | Visualizzazione dei numeri e del risultato finale |
| **Numeri** | `mat-flat-button` (Primary) | Pulsanti per l'inserimento delle cifre 0-9 |
| **Operazioni** | `mat-stroked-button` | Tasti per operatori (+, -, *, /) e calcolo (=) |
| **Reset** | `mat-flat-button` (Warn) | Funzione di pulizia totale della stringa di input |

---
*Progetto sviluppato per consolidare le competenze di integrazione tra framework logici e librerie di design professionale.*
