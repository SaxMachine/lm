# 📚 Simulazione Esame Spagnolo - 30 Minuti

Una pagina web interattiva per esercitarsi con una simulazione d'esame di spagnolo in 30 minuti.

**🌐 Demo Live:** [Apri la simulazione](./index.html)

---

## ✨ Caratteristiche

✅ **Timer globale 30 minuti** con avvisi di tempo scadente  
✅ **Organizzazione per tema** (Verbi, Preposizioni, Congiuntivo, Lessico)  
✅ **Mostra/Nascondi risposte** durante l'esame  
✅ **Conteggio progresso** (X esercizi completati su Y)  
✅ **Responsive** (funziona su mobile e desktop)  
✅ **Dark mode** automatico  
✅ **Nessun database** - tutto funziona offline  

---

## 🚀 Come Usare

### Opzione 1: GitHub Pages (Consigliato)

1. **Fork o clona il repository**
   ```bash
   git clone https://github.com/TUO_UTENTE/esercizi-spagnolo.git
   cd esercizi-spagnolo
   ```

2. **Attiva GitHub Pages**
   - Vai su **Settings** → **Pages**
   - Seleziona **Source: main** (o il branch che usi)
   - Salva

3. **Accedi alla pagina**
   ```
   https://TUO_UTENTE.github.io/esercizi-spagnolo
   ```

### Opzione 2: File Locale

Scarica `index.html` e apri direttamente nel browser:
```bash
open index.html
# oppure doppio-click sul file
```

---

## 📝 Come Aggiungere Esercizi

Apri `index.html` e trova la sezione `// ===== DATI ESERCIZI =====`

### Struttura Dati

```javascript
const exercises = {
    'Nome Tema': [
        {
            id: 1,
            title: 'Titolo esercizio',
            instructions: 'Istruzioni per il candidato',
            items: [
                { 
                    num: 1, 
                    text: 'Domanda con spazi ____', 
                    answer: 'risposta corretta' 
                },
                // ... altri item
            ]
        }
    ]
};
```

### Esempio Pratico

**Aggiungi un nuovo tema "Passato Prossimo":**

```javascript
'Passato Prossimo': [
    {
        id: 5,
        title: 'Coniuga i verbi al passato prossimo',
        instructions: 'Completa le frasi con il passato prossimo corretto',
        items: [
            { num: 1, text: '(Yo) ................. (hacer) los deberes ayer.', answer: 'he hecho' },
            { num: 2, text: 'Ellos ................. (venir) a las 5.', answer: 'han venido' },
            { num: 3, text: '¿(Tú) ................. (ver) a María?', answer: 'has visto' }
        ]
    }
]
```

---

## 🎨 Personalizzazione

### Cambia il Tempo dell'Esame

Nel file `index.html`, cerca questa riga:
```javascript
let timeLeft = 30 * 60; // 30 minuti in secondi
```

**Cambia in:**
- **45 minuti:** `45 * 60`
- **60 minuti:** `60 * 60`

### Cambia i Colori

Nel `<style>`:
```css
:root {
    --accent-info: #2563eb;        /* Blu (bottoni) */
    --accent-success: #10b981;     /* Verde (risposte) */
    --accent-warning: #f59e0b;     /* Arancione (avviso) */
    --accent-danger: #ef4444;      /* Rosso (urgente) */
}
```

**Palette libreria (salvia/marrone):**
```css
:root {
    --accent-info: #7a5c38;        /* Marrone */
    --accent-success: #6b8e5f;     /* Salvia */
    --accent-warning: #d4a574;     /* Beige scuro */
    --accent-danger: #c85a54;      /* Terracotta */
}
```

### Cambia il Titolo e le Statistiche

Modifica in `index.html`:
```html
<h1>📚 Simulazione d'Esame</h1>
<p>Prova la tua preparazione di spagnolo in 30 minuti</p>
```

---

## 📊 Struttura del File

```
esercizi-spagnolo/
├── index.html           ← File unico da ospitare
├── README.md           ← Questo file
└── .gitignore          ← (opzionale) Ignora file inutili
```

---

## 🔧 Tecnologie Usate

- **HTML5** - Struttura
- **CSS3** - Stili (con supporto dark mode)
- **Vanilla JavaScript** - Logica (senza dipendenze!)
- **GitHub Pages** - Hosting gratuito

---

## ✅ Checklist di Deployment

- [ ] Ho aggiunto tutti gli esercizi nel codice
- [ ] Ho testato il timer (inizia, conta, finisce)
- [ ] Ho verificato che "Mostra/Nascondi risposte" funziona
- [ ] Ho controllato il responsive su mobile
- [ ] Ho pushato il file su GitHub
- [ ] Ho abilitato GitHub Pages
- [ ] La pagina è raggiungibile al link pubblico

---

## 🐛 Troubleshooting

**Q: GitHub Pages non mostra la pagina**  
A: Assicurati che:
1. Il file si chiama `index.html`
2. È nella root del repository (oppure nella cartella `docs/`)
3. Pages è abilitato nelle Settings
4. Aspetta 1-2 minuti (GitHub Pages impiega tempo)

**Q: Il timer non parte quando clicco "Inizia"**  
A: Apri la console del browser (F12) e verifica che non ci siano errori JavaScript

**Q: Voglio cambiare il numero di minuti**  
A: Modifica `let timeLeft = 30 * 60;` nella sezione `<script>`

**Q: Le risposte non sono visibili quando clicco il bottone**  
A: Assicurati che ogni item abbia la proprietà `answer` nel codice

---

## 🎓 Per Insegnanti/Formatori

Se vuoi usare questa pagina con i tuoi studenti:

1. **Aggiungi più esercizi** dalla tua fonte
2. **Disabilita il bottone "Mostra risposte"** durante l'esame vero
3. **Salva i risultati** chiedendo agli studenti di fare uno screenshot finale

---

## 📄 Licenza

Libero di usare e modificare per scopi educativi.

---

**Ultima modifica:** Maggio 2026  
**Compatibilità:** Tutti i browser moderni (Chrome, Firefox, Safari, Edge)  
**Requisiti:** Solo un browser web (nessun server richiesto)
