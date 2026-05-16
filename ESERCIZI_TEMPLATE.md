# Template Esercizi - Estrai dal PDF e Compila

Questo file serve come **lista di controllo** per aggiungere gli esercizi dal PDF `Binder1.pdf`.

## 📋 Istruzioni

1. Leggi il PDF
2. Identifica ogni **tema/argomento**
3. Per ogni esercizio:
   - Copia il **titolo** → `title`
   - Copia le **istruzioni** → `instructions`
   - Estrai ogni **domanda singola** → `items[].text`
   - Copia la **risposta** dalla chiave risposte → `items[].answer`
4. Incolla nel blocco JavaScript dentro `index.html`

---

## ✅ Temi Già Presenti

- [x] **Verbi al futuro** (5 esercizi)
- [x] **Preposizioni** (6 esercizi)
- [x] **Congiuntivo vs Indicativo** (6 esercizi)
- [x] **Lessico Professionale** (5 esercizi)

**Totale esercizi attuali: 22**

---

## ⬜ Temi Da Aggiungere (da PDF)

### TEMA: Passato Prossimo
- [ ] **Titolo:** 
- [ ] **Istruzioni:** 
- [ ] **Numero domande:**
- [ ] **Domande estratte:**

```javascript
'Passato Prossimo': [
    {
        id: 5,
        title: 'TITOLO_QUI',
        instructions: 'ISTRUZIONI_QUI',
        items: [
            { num: 1, text: 'DOMANDA_1', answer: 'RISPOSTA_1' },
            { num: 2, text: 'DOMANDA_2', answer: 'RISPOSTA_2' },
            // ...
        ]
    }
]
```

---

### TEMA: Passato Imperfetto
- [ ] **Titolo:** 
- [ ] **Istruzioni:** 
- [ ] **Numero domande:**

```javascript
'Passato Imperfetto': [
    {
        id: 6,
        title: 'TITOLO_QUI',
        instructions: 'ISTRUZIONI_QUI',
        items: [
            { num: 1, text: 'DOMANDA_1', answer: 'RISPOSTA_1' },
        ]
    }
]
```

---

### TEMA: Presente Indicativo
- [ ] **Titolo:** 
- [ ] **Istruzioni:** 
- [ ] **Numero domande:**

```javascript
'Presente Indicativo': [
    {
        id: 7,
        title: 'TITOLO_QUI',
        instructions: 'ISTRUZIONI_QUI',
        items: [
            { num: 1, text: 'DOMANDA_1', answer: 'RISPOSTA_1' },
        ]
    }
]
```

---

### TEMA: Imperativo
- [ ] **Titolo:** 
- [ ] **Istruzioni:** 
- [ ] **Numero domande:**

```javascript
'Imperativo': [
    {
        id: 8,
        title: 'TITOLO_QUI',
        instructions: 'ISTRUZIONI_QUI',
        items: [
            { num: 1, text: 'DOMANDA_1', answer: 'RISPOSTA_1' },
        ]
    }
]
```

---

### TEMA: Subjuntivo
- [ ] **Titolo:** 
- [ ] **Istruzioni:** 
- [ ] **Numero domande:**

```javascript
'Subjuntivo Avanzato': [
    {
        id: 9,
        title: 'TITOLO_QUI',
        instructions: 'ISTRUZIONI_QUI',
        items: [
            { num: 1, text: 'DOMANDA_1', answer: 'RISPOSTA_1' },
        ]
    }
]
```

---

### TEMA: Pronuncia e Ortografia
- [ ] **Titolo:** 
- [ ] **Istruzioni:** 
- [ ] **Numero domande:**

```javascript
'Pronuncia e Ortografia': [
    {
        id: 10,
        title: 'TITOLO_QUI',
        instructions: 'ISTRUZIONI_QUI',
        items: [
            { num: 1, text: 'DOMANDA_1', answer: 'RISPOSTA_1' },
        ]
    }
]
```

---

## 📌 Come Inserire nel Codice

**Nel file `index.html`, trova questa sezione:**

```javascript
const exercises = {
    'Verbi al futuro': [ ... ],
    'Preposizioni': [ ... ],
    // ← AGGIUNGI QUI I NUOVI TEMI
};
```

**Aggiungi i nuovi temi così:**

```javascript
const exercises = {
    'Verbi al futuro': [ ... ],
    'Preposizioni': [ ... ],
    'Passato Prossimo': [
        {
            id: 5,
            title: 'Titolo',
            instructions: 'Istruzioni',
            items: [
                { num: 1, text: 'Domanda', answer: 'Risposta' },
            ]
        }
    ],
    // ... altri temi
};
```

---

## 🎯 Obiettivo Finale

**Target: 40-50 esercizi totali** (per una simulazione realistica di 30 minuti)

| Temi | Esercizi | Priorità |
|------|----------|----------|
| Verbi (Future, Past) | 15-20 | 🔴 Alta |
| Preposizioni | 5-10 | 🔴 Alta |
| Congiuntivo | 5-10 | 🟡 Media |
| Lessico | 5-10 | 🟡 Media |
| Vari | 5-10 | 🟢 Bassa |

---

## 🛠️ Checklist Completamento

- [ ] Ho estratto il tema dal PDF
- [ ] Ho copiato il titolo dell'esercizio
- [ ] Ho copiato le istruzioni
- [ ] Ho estratto tutte le domande numerando da 1
- [ ] Ho trovato le risposte corrette
- [ ] Ho formattato il codice JavaScript
- [ ] Ho incollato nel file `index.html`
- [ ] Ho testato che la simulazione funzioni
- [ ] Ho pushato le modifiche su GitHub

---

## 📖 Riferimento Veloce

**Numero totale esercizi nel PDF: ~265 (da 141 pagine)**

Seleziona i **40-50 migliori** per:
- Varietà di argomenti
- Difficoltà progressiva (facile → difficile)
- Mix di grammatica e lessico
