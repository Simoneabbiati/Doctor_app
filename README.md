# ✍️ Workshop: Scrivania Intelligente AI
**Guida allo sviluppo di un Writing Companion con Gemini 2.5 Flash**

Benvenuti in questo workshop. Oggi trasformeremo un'idea di design in un'applicazione web funzionante e pubblicata online, capace di interagire con l'intelligenza artificiale per potenziare la scrittura.

---

## 📅 Programma del Workshop (90 Minuti)

| Slot | Attività | Focus Tecnico |
| :--- | :--- | :--- |
| **00-15'** | **Setup & Architettura** | Google Canvas, Account GitHub, API Gemini |
| **15-30'** | **Layout & Modulo 01** | UI Minimalista (Tailwind) + Timer Pomodoro |
| **30-50'** | **Modulo 02: Freewriting** | Analisi del testo e Prompt Engineering |
| **50-70'** | **Modulo 03: Task Manager** | Scomposizione obiettivi (Logic AI) |
| **70-80'** | **Modulo 04: Suggerimenti** | Trigger dinamici (Invio) e Ghost Text |
| **80-90'** | **Deploy Finale** | Pubblicazione su GitHub Pages |

---

## 🏗️ 1. Architettura del Sistema

L'applicazione è un **Single Page Tool** sviluppato in React. 
- **Frontend:** Gestito tramite React (State Management) e Tailwind CSS (Styling).
- **Intelligenza Artificiale:** Utilizziamo l'endpoint nativo di Google Canvas per interrogare **Gemini 2.5 Flash**.
- **Integrazione:** La funzione `askAI` invia il testo dell'utente insieme a un *System Prompt* che definisce il comportamento dell'assistente.

---

## 💻 2. Sviluppo Moduli

### Modulo 01: Pomodoro dello Studioso (Frontend Generale)
È il cuore della gestione del tempo. 
- **Funzione:** Timer 25/5 per il Deep Work.
- **Dettaglio:** Prima di ogni sessione, l'utente dichiara la sua "Intenzione". Questo crea un impegno psicologico che l'IA userà nei moduli successivi.

### Modulo 02: Freewriting & Temi Chiave
Trasformiamo il "dump" di pensieri in struttura.
- **Cella Input:** Area di testo libera.
- **Cella Output:** Pannello laterale per i temi.
- **Prompt AI:** *"Identifica i 3 nuclei tematici principali di questo testo e riassumili in concetti da 2 parole."*

### Modulo 03: Scomponi il Mostro (Tasking)
L'IA come strumento di project management.
- **Input:** Un obiettivo macro (es: "Scrivere il capitolo 1").
- **Output:** Lista interattiva di micro-task da 15 minuti.
- **Prompt AI:** *"Agisci come un esperto di produttività. Dividi questo obiettivo in 5 azioni atomiche."*

### Modulo 04: Rientra nel Testo (Suggerimenti)
Superare il blocco della pagina bianca in tempo reale.
- **Meccanica:** Quando l'utente preme `Invio`, l'IA legge il paragrafo appena concluso.
- **Output:** Suggerisce l'incipit del paragrafo successivo.
- **Metriche:** Include un contatore di parole e un tachimetro della velocità di scrittura.

---

## 🚀 3. Istruzioni per il Deploy su GitHub

1. **Repository:** Crea un nuovo repository chiamato `scrivania-intelligente`.
2. **Upload:** Carica il file `index.html` creato durante il workshop.
3. **Settings:** Vai in `Settings` -> `Pages`.
4. **Build and Deployment:** Sotto *Branch*, seleziona `main` e clicca su `Save`.
5. **Live:** Dopo circa 60 secondi, la tua app sarà online all'indirizzo `https://tuo-nome.github.io/scrivania-intelligente/`.

---

## 📝 Note per gli Studenti
- Non è necessaria alcuna carta di credito.
- Il codice deve essere salvato costantemente.
- Sperimentate con i **System Prompts** per cambiare la "personalità" della vostra scrivania.

---
*Creato per il Workshop AI Writing Companion - Google Canvas Environment*
