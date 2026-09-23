<div align="center">

<img src="gorseller/codex-banner.png" alt="Numex Codex" width="100%">

# Numex Codex

### A coding agent that thinks in Turkish — for your editor, terminal and browser.

**Ask. It writes, runs and verifies — until the job is actually done.**

[🇹🇷 Türkçe](README.md) · 🇬🇧 **English**

</div>

---

Numex Codex is the coding agent of [Numex AI](https://numexai.com.tr), Türkiye's Turkish-first AI.
Tell it what you want in plain language; it **plans, writes, runs and tests** the code, and only says
"done" once it can **prove** it works. For complex work it doesn't act alone — it convenes a
**Council** of four specialists.

> 📌 This is Codex's showcase, documentation and community repo. Downloads:
> [codex.numexai.com.tr](https://codex.numexai.com.tr). Open-source SDK:
> [numex-sdk](https://github.com/mobilcep/numex-sdk).

## 🚪 Four doors, one agent

| | Where | Install |
|---|---|---|
| 🧩 **Codex IDE** | Windows desktop (VS Code based) | [Download](https://codex.numexai.com.tr) — v2.9.59, ~162 MB |
| 🧩 **VS Code extension** | Your existing VS Code | Install the extension + sign in via CLI |
| ⌨️ **Codex CLI** | Terminal | `npm i -g @numexai/cli` (v3.3.10) |
| 🌐 **Codex Web** | Browser | Nothing to install |

## 🏛️ The Council — four specialists, one task

Most coding agents grade their own homework: one model plans, writes, tests and declares success.
Codex hands complex tasks to a Council where every member has **one job and limited permissions**:

| Member | Job | Can write? |
|---|---|---|
| 📐 **Architect** | Folder structure, data model, per-file function plan | ❌ Plan only |
| 💻 **Coder** | Writes complete, working code — no stubs, no TODOs | ✅ **The only writer** |
| 🛡️ **Auditor** | First asks *"did we build the right thing?"*, then tests and verifies | ❌ Read & report only |
| 🎨 **Designer** | Polishes UI/UX | ⚠️ CSS/HTML only |

- **Single-writer rule** — only the Coder writes code, so agents never collide.
- **Off-topic plan check** — if the Architect's plan drifts from your request, the Coder follows *your request*, not the plan.
- **Right-sized team** — a one-line fix gets no council; a full-stack system gets all four. Token budget is checked up front (trivial ≈ 500 tokens … enterprise ≈ 30,000).
- **Summon it yourself** — *"konseyi topla"* ("gather the council").
- **Honest report** — a plain-language summary of who did what, including anything left unresolved.

→ [Full Council write-up (Turkish)](docs/konsey.md)

## 🚦 No "done" without proof — FinishGate

A task only closes with **live evidence**: an HTTP 200 from the running server, passing tests, or the
expected DOM in a headless browser. Otherwise the agent returns to a **self-healing loop**. If it gets
stuck, a stuck-detector hands control back to you.

## 🔀 Four modes

**Chat** (explain, answer) · **Plan** (no edits, just a roadmap) · **Autonomous** (plan → approve →
apply → verify) · **Bug Hunter** (root cause from logs and output).

## ⌨️ CLI highlights

```bash
numex "build a dark-themed todo app"
numex plan "add a payment module"      # plan only
numex mission "make the tests pass"    # long-running autonomous mission in sandboxed worktrees
numex undo                             # roll back the last turn
numex --offline "…"                    # local Ollama, no internet
numex uzak install                     # control your PC from your phone
```

Surgical diff-based patching · background process error interception · BM25 + AST code index · MCP
client · live tree progress.

## 🧠 Transparent memory

Every project gets a readable `.numex/` folder: RAG index, **audit trail** of every action, undo
checkpoints, learned errors, mission state and token usage. → [docs/numex-klasoru.md](docs/numex-klasoru.md)

## 🤝 Community

Bugs and ideas → [Issues](../../issues/new/choose) · Show what you built → [Discussions](../../discussions) ·
Security → **destek@numexai.com.tr**
