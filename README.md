# Workshop: Sviluppare la Scrivania Intelligente con l'AI
### Guida metodologica alla creazione di un Writing Companion con Gemini 2.5 Flash

---

## Panoramica del Progetto
L'obiettivo di questo workshop è trasformare un'idea di design in un'applicazione web funzionante e pubblicata online. Gli studenti impareranno a integrare modelli linguistici avanzati (LLM) all'interno di un'interfaccia utente moderna per potenziare il flusso creativo e la produttività.

**Target:** Sviluppatori junior, designer e appassionati di AI.
**Durata:** 90 Minuti (Sessione intensiva).
**Tecnologie:** React, Tailwind CSS, Google Gemini 2.5 Flash, GitHub Pages.

---

## 1. Architettura e Configurazione (20 min)
*Comprendere il flusso dei dati e preparare l'ecosistema di sviluppo.*

### Fondamenta Tecniche
* Ambiente: Configurazione di Google Canvas come IDE rapido.
* Integrazione Nativa: Analisi del modello gemini-2.5-flash-preview-09-2025.
* Sicurezza e Autenticazione: Gestione dell'autenticazione tramite API Key automatica (Zero-Config).

### Il Core Engine: La Funzione askAI
Implementazione di un'architettura stateless per le chiamate API:
1. Costruzione del Payload: Definizione del corpo della richiesta JSON.
2. System Prompting: Iniezione di istruzioni comportamentali persistenti.
3. Gestione della Risposta: Parsing dei dati e gestione degli errori di rete.

---

## 2. Design di Sistema e Modulo 01 (20 min)
*Costruire l'interfaccia e implementare la logica temporale.*

### UI/UX: Layout Paper Design
* Grid System: Struttura a griglia asimmetrica con Tailwind CSS.
* Estetica: Palette cromatica scura con accenti crema (#d1c9b8) per favorire il focus.

### Modulo 01: Pomodoro dello Studioso
* Sfida: Gestione degli stati temporali in React (useState, useEffect).
* Funzionalità:
    * Countdown dinamico (25/5 minuti).
    * Persistenza dello stato per l'Intenzione di Sessione.
* Obiettivo: Familiarizzare con il ciclo di vita dei componenti prima dell'integrazione IA.

---

## 3. Livelli di Intelligenza (40 min)
*Potenziare l'editor con moduli di analisi e generazione.*

### Modulo 02: Analisi Tematica (Freewriting)
* Prompt Engineering: Analizza il testo e identifica i nuclei tematici principali in forma di tag.
* Frontend: Area di input dedicata e sidebar dei metadati.

### Modulo 03: Scomponi il Mostro (Tasking)
* Algoritmo di Scomposizione: Trasformazione di obiettivi macro in micro-azioni atomiche da 15 minuti.
* Frontend: Generazione dinamica di liste di controllo basate su output AI.

### Modulo 04: Flow Engine (Suggerimenti)
* Metriche in tempo reale: Implementazione di un tachimetro di velocità (WPM) e contatore parole.
* Predictive UX: All'evento onKeyPress (Invio), l'IA analizza il contesto e suggerisce l'incipit del paragrafo successivo.

---

## 4. Deployment e Distribuzione Globale (10 min)
*Rendere l'applicazione accessibile al mondo.*

1. Sincronizzazione Repository: Inizializzazione di un repository Git su GitHub.
2. Hosting degli Asset: Caricamento del file index.html.
3. CI/CD: Attivazione di GitHub Pages per il deployment automatico.
4. Verifica: Test finale della connettività API in ambiente di produzione.

---

## Roadmap Operativa

| Orario | Fase | Attività Principale |
| :--- | :--- | :--- |
| 00-15' | INIT | Setup Account e Architettura API |
| 15-30' | BASE | Layout Responsive e Timer Pomodoro |
| 30-50' | LOGIC I | Modulo Freewriting (Integrazione Gemini) |
| 50-70' | LOGIC II | Modulo Task Manager (Dati Strutturati) |
| 70-80' | FLOW | Suggerimenti Dinamici e Metriche |
| 80-90' | LIVE | Deploy su GitHub Pages e Q&A |

---
> "La tecnologia migliore è quella che scompare per lasciare spazio alla creatività."
