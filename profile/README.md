# MayAI

**Costruiamo soluzioni intelligenti per chi fa impresa in Italia.**

Aiutiamo aziende e professionisti ad automatizzare i loro processi con agenti AI su misura, integrati nei sistemi che usano ogni giorno. Su questo profilo pubblichiamo gli strumenti open-source che costruiamo e usiamo internamente.

## ⭐ In evidenza — BandiRadar

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

## ⭐ Featured — BandiRadar

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
