# The Dated Record Method & Semantic Role Logic ("Case Filter" v1.3)

> **[Русская версия документации (README.md)](./README.md)**

[![DOI](https://img.shields.io/badge/DOI-10.5281%2Fzenodo.24516089-blue)](https://doi.org/10.5281/zenodo.24516089)
[![nRIS](https://img.shields.io/badge/nRIS-No._852--137--831-green)](https://xn--e1axe4b.xn--h1apes.xn--p1ai/object/?id=27428445211064eee31ca68e7b127b3d43c62ffbaa8c710e604d16582c0e440a&channel=media)
[![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC_BY--NC_4.0-lightgrey.svg)](./LICENSE.md)

**A deterministic structural guardrail against LLM hallucinations, hidden passive voice ("Empty Seat"), and linguistic traps in contracts, news, and reports.**

---

### Try Live in Your Browser (No Sign-Up or Installation Required)

* **[Open All-in-One Studio (MACROS-OS Studio EN)](https://irinavetlugina.github.io/dated-record-case-filter/macros_os_studio_en.html)** — automated structural X-ray for contracts, bureaucratic replies, news, and AI outputs with ready-to-use "HOW IT SHOULD BE" rewrites (runs locally in your browser)
* **[Open Interactive Observer Trainer (18 Cells EN)](https://irinavetlugina.github.io/dated-record-case-filter/observer_trainer_en.html)** — step-by-step interactive trainer for verifying statements
* **[Открыть студию «Всё в одном» (RU)](https://irinavetlugina.github.io/dated-record-case-filter/macros_os_studio.html)** | **[Открыть Пульт Наблюдателя (RU)](https://irinavetlugina.github.io/dated-record-case-filter/observer_trainer_ru.html)**

---

### IP Priority, Scientific Archive & License

* **Author & Copyright Holder:** Irina Vladimirovna Vetlugina (Samara, Russia)
* **State IP Deposit (n'RIS):** Certificate **No. 852-137-831** dated November 20, 2026 (core specification `v1.2`)
* **CERN International Scientific Archive (Zenodo):** [https://doi.org/10.5281/zenodo.24516089](https://doi.org/10.5281/zenodo.24516089)
* **Terms of Use:** The core specification, Python/MCP code, browser studios, and open prompt engines are free for personal, academic, and educational use (`CC BY-NC 4.0`). For commercial licensing, API/MCP integration, and enterprise deployment, contact: **polutshe@mail.ru**

---

## 1. REPOSITORY FILE MAP

### Standalone Browser Studios (HTML / GitHub Pages)
1. **`macros_os_studio_en.html`** / **`macros_os_studio.html`** — all-in-one browser workstation (Autopilot, Contracts, News/Replies, AI Mirror + "HOW IT SHOULD BE" rewrite templates).
2. **`observer_trainer_en.html`** / **`observer_trainer_ru.html`** — interactive Observer Trainer covering 18 structural failure modes.

### Text Action Engines for Any LLM (`macros-os-versions/` folder)
3. **[`macros-os-versions/macro-os-v8.0-autopilot.md`](./macros-os-versions/macro-os-v8.0-autopilot.md)** — **"Autopilot" (1-Step Zero-Command Start)**: automatically detects document type, runs a 5-role structural check, and outputs a clean rewrite.
4. **[`macros-os-versions/macro-os-v9.5-complete.md`](./macros-os-versions/macro-os-v9.5-complete.md)** — **"Four-Track Complete Console"**: lightweight engine with dormant modes for news (`ONION`), contracts (`CONSTRUCTOR`, `PAIR-CHECK`, `DEVIL'S ADVOCATE`), AI auditing (`MIRROR`, `CHAIN`, `RESOURCE`), and problem analysis (`NAVIGATOR`, `DEGENERATION`).
5. **[`macros-os-versions/macro-os-v7.0-tribunal.md`](./macros-os-versions/macro-os-v7.0-tribunal.md)** — **"Tribunal & Arbitrage"**: adversarial three-contour review (Prosecutor / Defender / Judge) and cross-model verification of other LLMs (`ARBITRAGE`).
6. **`case-filter-v1.3-en.md`** / **`padezhny-filtr-v1.3.md`** — ultra-lightweight core specification (English and Russian versions).

### Infrastructure & Code (Python / MCP)
7. **`case_filter_mcp_server.py`** — **Model Context Protocol (MCP) Server** for Claude Desktop, Cursor, Windsurf, and enterprise AI agents. Blocks outgoing messages and contract approvals containing passive voice, unanchored metrics, or rubber deadlines (`< 0.5 ms` response time, zero external dependencies).
8. **`case_compiler.py`** — standalone deterministic Python compiler for checking texts and files without LLM calls.

---

## 2. QUICK START IN ANY AI CHAT (NO CODING REQUIRED)

1. Open a new chat in ChatGPT, Claude, Gemini, or DeepSeek.
2. Copy the contents of your chosen file from the **`macros-os-versions/`** folder (beginners should start with **`macro-os-v8.0-autopilot.md`**; for full multi-track capabilities, choose **`macro-os-v9.5-complete.md`**) and paste it as your first message.
3. In **Autopilot v8.0**, simply paste any text without commands — the system classifies and audits it automatically.
4. In **Complete Console v9.5**, targeted commands are available on demand.

---

## 3. QUICK START FOR DEVELOPERS (MCP SERVER)

To connect Case Filter as a deterministic guardrail in **Claude Desktop** or **Cursor**, add this to your configuration file (`claude_desktop_config.json`):

```json
{
  "mcpServers": {
    "case-filter": {
      "command": "python3",
      "args": ["/absolute/path/to/folder/case_filter_mcp_server.py"]
    }
  }
}
```

After restarting, your AI agent gains three system tools:
* `verify_statement` — blocks hallucinations, passive voice, and unanchored metrics before sending.
* `audit_contract_clause` — checks contract clauses for rubber deadlines and hidden "Empty Seat" traps.
* `get_cell_registry` — taxonomy reference for failure modes `Cells 1–18 + R6`.

---

## 4. LICENSE & COPYRIGHT

**Dual License — Copyright © 2026 Irina Vetlugina (Samara, Russia).**  
Core methodology IP priority is registered in **n'RIS No. 852-137-831 (November 20, 2026)**.

1. **Non-Commercial Use (`CC BY-NC 4.0`):** free for personal, academic, and educational purposes with mandatory author attribution.
2. **Commercial Use:** embedding into SaaS products, corporate API gateways, paid consulting, or commercial services requires a separate commercial license agreement with the author (**polutshe@mail.ru**).
