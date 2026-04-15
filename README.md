# 🖥️ dashboard-admin skill

Una skill per Claude che genera dashboard admin moderne, production-grade, con React + Tailwind CSS.
Costruita a partire da pattern reali, copre tutto il necessario — dal layout shell ai grafici — con supporto nativo per tema dark/light switchabile.

---

## ✨ Cosa fa

Quando installi questa skill, Claude è in grado di:

- Costruire da zero una **dashboard admin completa** con sidebar, header, pagine e componenti
- Scegliere automaticamente lo **stile visivo** più adatto al contesto del tuo progetto
- Generare codice **production-ready** con Tailwind CSS, accessibilità e responsive inclusi
- Applicare **pattern coerenti** tra tutti i componenti (spacing, colori, tipografia)

Basta descrivere cosa vuoi — Claude capisce il contesto e produce codice funzionante.

---

## 🧩 Componenti inclusi

| Componente | Dettagli |
|---|---|
| **Sidebar** | Collassabile, tooltip su icone, sezioni categorizzate, upsell card, avatar utente |
| **Header** | Sticky, breadcrumb, barra di ricerca con shortcut `⌘K`, notifiche, theme toggle |
| **Card KPI** | Trend indicator, sparkline inline, icona pastello, variante orizzontale |
| **Tabella dati** | Sort multi-colonna, ricerca full-text, paginazione, badge di stato |
| **Grafici** | Area, Bar orizzontale, Donut/Pie con legenda, Sparkline, Radial progress |
| **Form** | Validazione con React Hook Form + Zod, feedback errori inline |
| **Modal** | Focus trap, chiusura con Escape, overlay, animazione zoom |
| **Toast** | Stack di notifiche, auto-dismiss, varianti success/error/warning/info |
| **Skeleton loader** | Per stati di caricamento asincrono |

---

## 🎨 5 Stili Visivi

La skill riconosce il contesto e applica lo stile più adatto. Puoi anche specificarlo esplicitamente.

### 🖤 Minimalista / Editorial
Bianco puro, grafica monocromatica, nessuna distrazione. Numeri grandi, bordi sottili, zero ombre.
**Ideale per**: tool interni B2B, gestione team, SaaS enterprise.

### 📚 Documentation / Dev-Oriented
Layout a L, callout con bordo sinistro colorato, codice inline in badge monospace.
**Ideale per**: portali developer, knowledge base, admin con navigazione profonda.

### 🟢 Professionale / Analytics
Sidebar scura + main chiara (contrasto forte), accent teal, KPI orizzontali, sezioni nav categorizzate.
**Ideale per**: analytics, monitoring, dashboard operative con molti dati.

### 💜 Morbido / SaaS Modern
Sfondo bianco caldo `#F4F7FE`, viola primario, angoli arrotondati, ombre morbide, upsell card in sidebar.
**Ideale per**: SaaS consumer, prodotti AI, startup, app creative.

### 🔵 Dark / Futuristico
Navy scuro `#0B1437`, azzurro elettrico, icone quadrate nelle card, elemento decorativo 3D, FAB settings.
**Ideale per**: fintech, crypto, analytics enterprise, prodotti premium.

---

## 🗂️ Struttura della Skill

```
dashboard-admin/
├── SKILL.md                    # Istruzioni principali + architettura
└── references/
    ├── styles.md               # 5 stili visivi con palette e pattern ⭐
    ├── layout.md               # Sidebar, Header, Breadcrumb
    ├── components.md           # KPI, Tabelle, Form, Modal, Toast
    ├── charts.md               # Grafici con Recharts
    └── theming.md              # Dark/Light mode, CSS vars, animazioni
```

---

## ⚙️ Stack Tecnologico

```json
{
  "framework":    "React (pattern trasferibili a Vue, Angular, Svelte)",
  "styling":      "Tailwind CSS + CSS Variables HSL",
  "ui":           "shadcn/ui",
  "charts":       "Recharts",
  "icons":        "lucide-react",
  "forms":        "react-hook-form + zod",
  "routing":      "react-router-dom v6",
  "state":        "zustand o Context API",
  "animations":   "framer-motion + tailwindcss-animate",
  "tables":       "tanstack/react-table v8"
}
```

---

## 🚀 Installazione

### Claude Code (terminale)
```bash
claude skill install dashboard-admin.skill
```

### Manuale
Decomprimi il file `.skill` (è un archivio zip) e posiziona la cartella `dashboard-admin/` nella directory delle skill del tuo ambiente Claude.

---

## 💬 Come usarla

Una volta installata, basta fare richieste naturali a Claude:

```
"Crea una dashboard admin per gestire gli utenti con sidebar e tema dark"

"Fammi un pannello di controllo e-commerce con grafici di vendita"

"Costruisci un admin panel stile SaaS moderno con card KPI e tabella ordini"

"Voglio una dashboard analytics professionale con molti dati"
```

Claude riconosce automaticamente il contesto, sceglie lo stile adatto e genera il codice completo.

---

## 🔧 Personalizzazione

Per adattare la skill ai tuoi progetti, puoi modificare:

- **`references/styles.md`** — aggiungi i tuoi stili personalizzati o modifica le palette
- **`references/theming.md`** — cambia le CSS variables con i colori del tuo brand
- **`SKILL.md`** — aggiusta il trigger o aggiungi regole specifiche al tuo workflow

---

## 📄 Licenza

Skill creata con Claude. Libera da usare e modificare nei tuoi progetti.
