# MayAI

**Costruiamo soluzioni intelligenti per chi fa impresa in Italia.**

Aiutiamo aziende e professionisti ad automatizzare i loro processi con agenti AI su misura, integrati nei sistemi che usano ogni giorno. Su questo profilo pubblichiamo gli strumenti open-source che costruiamo e usiamo internamente.

## ⭐ In evidenza

### 📏 ItalBizBench — il metro per gli agenti

**[`italbizbench`](https://github.com/mayai-it/italbizbench)** · il benchmark open-source che misura quanto bene un agente AI svolge **davvero** il lavoro fiscale-amministrativo di una PMI italiana: fatture, scarti SDI, reverse charge, split payment, imposta di bollo.

- **88 task con oracolo deterministico** — niente LLM-giudice; tre livelli di difficoltà, inclusi casi *adversarial* dove l'agente corretto si ferma e chiede conferma
- **Scoring su 4 assi** — correttezza, efficienza (tool-call, token, **costo in €**), sicurezza, calibrazione (Brier, ECE, reliability curve)
- **Statistica onesta** — pass-rate con IC al 95% (bootstrap + Wilson): due agenti sono "diversi" solo se gli intervalli non si sovrappongono
- Sandbox in-memory con simulatore SDI (*mai API live*, solo dati sintetici) · leaderboard HTML statica per GitHub Pages · regole fiscali tracciate su fonti · MIT

*In produzione la sandbox si sostituisce con `fatture-cli` / `pec-cli` via MCP: il benchmark misura gli agenti sugli stessi strumenti con cui poi lavorano.*

### 📡 BandiRadar

**[`bandiradar`](https://github.com/mayai-it/bandiradar)** · motore open-source che monitora le opportunità di finanziamento pubblico italiane (gare, bandi, incentivi), le normalizza in un unico modello e le classifica rispetto al profilo di un'azienda.

- **Matcher a due stadi** — prefiltro deterministico + rilevanza LLM, con un fallback offline che gira *senza chiavi*
- **Fonti live, senza API key** — TED (gare UE aperte) e incentivi.gov.it (incentivi nazionali)
- **Benchmark storici ANAC** — valore tipico di aggiudicazione e scostamenti, per dare contesto a ogni opportunità
- CLI + **MCP server** nativo · gira offline sui dati di esempio, zero segreti · MIT

## 🛠️ CLI tools

Le linee di comando che usiamo internamente per dare agli agenti AI un accesso pulito e *context-efficient* alle API. Ogni CLI include un **MCP server** nativo — usabile direttamente in Claude Desktop, Cursor e altri agent, senza subprocess o parsing JSON.

| CLI | Cosa fa |
|---|---|
| [`fatture-cli`](https://github.com/mayai-it/fatture-cli) | Wrapper dell'API di Fatture in Cloud |
| [`pec-cli`](https://github.com/mayai-it/pec-cli) | IMAP/SMTP per caselle PEC |
| [`linkedin-cli`](https://github.com/mayai-it/linkedin-cli) | Accesso programmatico a LinkedIn per agenti |

🌐 [**mayai.it**](https://mayai.it)

---

# MayAI

**We build AI that works the way Italian businesses do.**

We help companies and professionals automate their processes with custom AI agents, integrated with the systems they use every day. This profile hosts the open-source tools we build and use internally.

## ⭐ Featured

### 📏 ItalBizBench — the yardstick for agents

**[`italbizbench`](https://github.com/mayai-it/italbizbench)** · the open-source benchmark that measures how well an AI agent **actually** does the fiscal and administrative work of an Italian SME: invoices, SDI rejections, reverse charge, split payment, stamp duty.

- **88 tasks with deterministic oracles** — no LLM-as-judge; three difficulty tiers, including *adversarial* cases where the correct agent stops and asks for confirmation
- **4-axis scoring** — correctness, efficiency (tool calls, tokens, **cost in €**), safety, calibration (Brier, ECE, reliability curve)
- **Honest statistics** — pass-rate with 95% CIs (bootstrap + Wilson): two agents are "different" only if their intervals don't overlap
- In-memory sandbox with an SDI simulator (*never a live API*, synthetic data only) · static HTML leaderboard for GitHub Pages · fiscal rules tracked against sources · MIT

*In production the sandbox is swapped for `fatture-cli` / `pec-cli` over MCP: the benchmark measures agents on the same tools they then work with.*

### 📡 BandiRadar

**[`bandiradar`](https://github.com/mayai-it/bandiradar)** · an open-source engine that monitors Italian public funding opportunities (tenders, grants, incentives), normalizes them into one canonical model, and ranks them against a company profile.

- **Two-stage matcher** — deterministic prefilter + LLM relevance, with an offline fallback that runs with *zero secrets*
- **Live sources, no API key** — TED (open EU tenders) and incentivi.gov.it (national incentives)
- **Historical ANAC benchmarks** — typical award value and outliers, for context on every opportunity
- CLI + native **MCP server** · runs offline on sample data, zero secrets · MIT

## 🛠️ CLI tools

The command-line tools we use internally to give AI agents clean, *context-efficient* access to APIs. Each CLI ships a native **MCP server** — use it directly in Claude Desktop, Cursor, and other agents, without subprocess calls or JSON parsing.

| CLI | Purpose |
|---|---|
| [`fatture-cli`](https://github.com/mayai-it/fatture-cli) | Fatture in Cloud API wrapper |
| [`pec-cli`](https://github.com/mayai-it/pec-cli) | IMAP/SMTP for Italian certified mail (PEC) |
| [`linkedin-cli`](https://github.com/mayai-it/linkedin-cli) | Programmatic LinkedIn access for agents |

🌐 [**mayai.it**](https://mayai.it)
