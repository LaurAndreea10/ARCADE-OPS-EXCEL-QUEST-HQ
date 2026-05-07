# ARCADE OPS: EXCEL QUEST — v3

> **Un univers gamificat care combină puzzle-uri Excel, prioritizare operațională și un hub arcade futurist într-o experiență single-file.**

Built by Laura Andreea — RO/EN bilingual portfolio project demonstrând product thinking, UX design, frontend engineering și visual identity.

---

## 📦 Structura proiectului

```
arcade-ops-excel-quest/
├── index.html          # Aplicația principală (~240KB, 6,600+ linii)
├── about.html          # Landing page de prezentare
├── case-study.html     # Case study detaliat (process + decisions + lessons)
└── README.md
```

**Zero dependențe externe.** Trei fișiere HTML self-contained.

---

## ⚡ Ce e nou în v2

### 🔊 Sound design
Engine audio sintetizat cu **Web Audio API** — zero fișiere externe:
- Click-uri subtile pe butoane
- Arpeggii ascendente la success
- Combo escalation (frequency creste cu combo-ul)
- Boss hit cu noise burst
- Rank-up flourish (4 note triumfătoare)
- Buton de mute în HUD (♪ / ⊘)

### 🔥 Daily Challenges + Streak System
- **3 provocări noi** generate determinist din data zilei
- Streak counter cu **bonus XP până la +50%**
- Timer real-time până la reset
- 6 tipuri de challenges: triage perfect, formula streak, workflow first-try, combo, missions count, high score

### ✨ Customization Station
- **6 avatar skins** unlock-abile cu coins (Neon Clasic, Cyan Pulse, Lime Circuit, Amber Flame, Gold Elite, Prizm Master)
- **5 neon themes** (Magenta Ops, Cyber Blue, Toxic Lime, Sunset Hunt, Matrix Green)
- Theme-ul schimbă paleta întregului joc **live** (CSS variables)
- Avatar-ul se aplică și în Hub și în Profile

### 📚 Conținut extins
- Triage Rush: **12 → 25 task-uri** (Stripe webhook, GDPR, vendor disputes, DDoS, etc.)
- Formula Lab: **8 → 21 puzzle-uri** (VLOOKUP, INDEX-MATCH, ROUND, MAX, IFERROR, LEN, TEXT, TRIM, TODAY, LEFT/RIGHT, AND/OR, COUNTIF criteria)

### 🎓 Onboarding tutorial
Overlay 5-step pentru first-time users:
1. Welcome → context-ul jocului
2. Triage Rush → 4 acțiuni + keyboard shortcuts
3. Formula Lab → puzzle-uri + tipuri
4. Progression → XP, ranks, combo
5. Districts & Boss → world map + Queue Hydra

Skip option oricând. Detectează automat first-time vs returning user.

### 🌐 Landing page (`about.html`)
Pagină separată orientată spre recruiteri:
- Hero cu shimmer animation
- 4 pillars (concept overview)
- 9 systems (toate feature-urile)
- 4 skill columns (Product / UX / Frontend / Visual)
- Tech stack badges
- CTA card
- Mobile responsive

### 🏆 Achievements extinse (12 → 33)
Sistem extins de badges cu **4 tier-uri** și design diferențiat:
- **8 Common** (gri) — early game (Prima Misiune, Triage Novice, Combo 5x, Primii 100)
- **11 Rare** (cyan) — comportament consistent (Perfect Run, Streak x3, Stylist, Operative)
- **8 Epic** (magenta) — skill mare (Hydra Slayer, Excel Prodigy, Week Warrior, High Roller)
- **6 Legendary** (gold cu shimmer animation) — endgame prestige (Master Operator, Hydra Nemesis, Combo 20x, Centurion, Completionist)

Verificare retroactivă: la deschiderea Profile-ului, achievements deja calificate sunt deblocate automat.

### 📄 Case Study (`case-study.html`)
Document recruiter-facing detaliat care prezintă procesul complet:
- **01 Problem** — de ce încă un proiect de portofoliu
- **02 Concept** — 4 piloni care au definit fiecare decizie
- **03 Key Decisions** — single-file vs modular, SFX sintetizate vs samples, RO/EN bilingv, onboarding 5-step
- **04 Challenges** — game feel cu zero biblioteci, balansarea progresiei, state management fără Redux
- **05 By the numbers** — 6,600+ linii, 240KB, 0 dependențe
- **06 Lessons learned** — 5 lecții transferable
- **07 What's next** — roadmap

Bilingv RO/EN cu toggle live, typography mix Orbitron + Lora serif italic pentru un ton mai "editorial" decât gameplay-ul.

### 📊 Stats & Analytics
Dashboard de performanță cu **3 grafice SVG vanilla** (zero deps):
- **Chart 1 — Evoluție XP:** linie cumulativă cu animație draw-in pe ultimele 15 misiuni
- **Chart 2 — Accuracy / Mode:** bar chart cu 4 culori per mode (Triage orange, Formula cyan, Workflow lime, Boss magenta)
- **Chart 3 — Distribuție Combo:** histogram cu 6 buckets (0, 1-2, 3-4, 5-7, 8-10, 11+) și paletă progresivă

**6 summary tiles:** Total Misiuni, Accuracy Medie, Cel Mai Bun Combo, Total XP, Runs Perfecte, Boss Defeated.

**Mission log** cu cap la 50 misiuni recente, persistat în localStorage. Empty state pentru sub 3 misiuni jucate.

---

## 🎮 Mecanici principale

| Modul | Conținut | Mecanică |
|-------|----------|----------|
| **Triage Rush** | 25 task-uri | Resolve / Escalate / Defer / Assign |
| **Formula Lab** | 21 puzzle-uri | Multiple choice cu hints |
| **Workflow Builder** | 5 procese | Drag-to-reorder steps |
| **Crisis Room** | Mixed mode | Triage + boss elements |
| **Boss: Queue Hydra** | 3 faze | Multiplicare la greșeală |

---

## 🎯 Progresie

- **8 ranguri** de la Trainee → Master Operator
- **12 achievement-uri** (badges)
- **6 districte** unlock-abile progresiv
- **XP + Coins** economy
- **localStorage** persistence (key: `arcade-ops-excel-quest-v1`)

---

## ⌨️ Keyboard shortcuts

**Triage Rush:** `1` `2` `3` `4` (sau `R` `E` `D` `A`)
**Formula Lab:** `A` `B` `C` `D` (sau `1-4`)
**Global:** `Esc` pentru exit

---

## 🚀 Deployment pe GitHub Pages

1. Creează repo nou: `arcade-ops-excel-quest`
2. Push ambele fișiere (`index.html` și `about.html`)
3. Settings → Pages → Source: `main` branch, root folder
4. Demo va fi disponibil la: `https://laurandreea10.github.io/arcade-ops-excel-quest/`
5. Landing page la: `https://laurandreea10.github.io/arcade-ops-excel-quest/about.html`

**Pentru CV/LinkedIn:** trimite link-ul către `about.html` (este orientat spre cititor) și include și link-ul direct către `index.html` pentru cei care vor să joace direct.

---

## 🛠️ Tech stack

- HTML5 / CSS3 / Vanilla JavaScript
- Web Audio API (SFX)
- localStorage (persistence)
- CSS custom properties (theming)
- Google Fonts (Orbitron, Rajdhani, JetBrains Mono)
- Zero build tools, zero npm packages

---

## 📊 Metrici

- **~232 KB** un singur fișier (index.html)
- **~22 KB** landing page (about.html)
- **6,500+** linii de cod
- **0** dependențe externe
- **2** limbi (RO + EN)
- **51** task-uri și puzzle-uri unice
