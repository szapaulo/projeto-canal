# 🐙 POLVO 4.1 — Central Brain

> An autonomous content creation system for dark channels. Discovery → Intelligence → Agents → Production → Distribution → Metrics → Learning → Scale.

---

## Architecture

```
DATA → INTELLIGENCE → AGENTS → AUTOMATION → CREATION → PRODUCTION → DISTRIBUTION → METRICS → LEARNING → MEMORY → SCALE ↺
```

The Polvo is not a set of AI tools. It is a **closed-loop agentic system** that finds content opportunities, understands why they work, creates new pieces, publishes, measures results, and uses data to improve the next cycle.

### Core Pipeline

```
         🔎 DISCOVERY (Viral Hunter)
              ↓
         🧬 VIRAL ANALYST (DNA breakdown)
              ↓
         🎯 ANGLE + HOOK agents
              ↓
         ✍️ WRITER → 🛡️ RED TEAM
              ↓
         🎬 CREATIVE DIRECTOR (storyboard)
              ↓
         🎨 VISUAL (Kling/Higgsfield) + 🎙️ VOICE (ElevenLabs)
              ↓
         🏭 MoneyPrinterTurbo (assembly)
              ↓
         ✂️ CapCut → 👁️ QA
              ↓
         🚀 DISTRIBUTION (TikTok/YT/IG/FB)
              ↓
         📊 ANALYTICS → 🧠 LEARNING → PATTERN MINER → OBSIDIAN → NEW CYCLE
```

---

## Directory Structure

| Dir | Purpose | Lang |
|---|---|---|
| `00_Start_Here/` | Dashboard, quickstart for AI agents, entry MOC | EN |
| `01_Planejamento/` | Strategy, budget, stack definition, context, glossary | pt-BR |
| `02_Estudo/` | Research on tools, platforms, concepts, algorithms | pt-BR |
| `03_Memoria/` | Accumulated knowledge: niches, virals, hooks, themes, angles, formats, patterns, experiments | pt-BR |
| `04_SOPs/` | Standard Operating Procedures (step-by-step guides) | EN |
| `05_Prompts/` | Versioned prompt library organized by agent type | EN |
| `06_Agentes/` | Agent definitions: responsibilities, inputs, outputs, tools | EN |
| `07_Producao/` | Production pipeline: ideas → scripts → videos → published | pt-BR |
| `08_Metricas/` | Analytics dashboard, learnings, A/B test results | pt-BR+EN |
| `09_Automacoes/` | n8n workflows, Python scripts, MCP configurations | EN |
| `10_Changelog/` | Project history: decisions, milestones, architecture changes | EN |
| `99_Templates/` | Obsidian note templates with frontmatter | mixed |
| `Assets/` | Images, PDFs, media attachments | — |

---

## Golden Rules

1. **Budget ceiling: R$300/month.** Never exceed without explicit approval.
2. **Core paid: Claude Pro + CapCut Pro (~R$170-190).** Remainder is compute fund.
3. **Log every decision** in `10_Changelog/Changelog.md` before making major changes.
4. **This repo is memory, not runtime.** Agents execute via n8n + MCP.
5. **Everything is versioned.** Prompts, SOPs, scripts, agent definitions.
6. **NO copyrighted material.** All content must be original or properly licensed.

---

## Current Status

**Phase:** Study & Planning

- Stack Polvo 4.1 defined
- Budget plan finalized (R$300/month)
- Initial niche/format research started
- Production has NOT started yet
- No channels created yet

### Immediate Next Actions
- [ ] Create YouTube and TikTok accounts
- [ ] Define final niche + format combination
- [ ] Install and configure MoneyPrinterTurbo
- [ ] Set up n8n self-hosted
- [ ] Create first SOP (video creation flow)
- [ ] Build first agent definitions
- [ ] Produce first test video

---

## Token Budget Guide (for AI Agents)

When operating in this repository, follow this reading order to minimize token usage:

| Step | File | Why |
|---|---|---|
| 1 | `README.md` | Mission, architecture, rules, status |
| 2 | `00_Start_Here/Quickstart_Agent.md` | Entry protocol and conventions |
| 3 | `01_Planejamento/Planejamento de Stack.md` | Full stack and agent architecture |
| 4 | `10_Changelog/Changelog.md` (last 3 entries) | Recent decisions and context |
| 5 | Task-specific files only | Read only what the task requires |

**Skip** unless explicitly needed: `03_Memoria/*`, `08_Metricas/*`, `Assets/*`, any file with `status: arquivado` in frontmatter.

---

## Obsidian Features in Use

| Feature | Location | Purpose |
|---|---|---|
| Graph View | Global | Visual navigation of linked notes |
| Dataview | `Dashboard.md` | Dynamic queries for production status |
| Kanban | `Kanban.md` | Project tracking board |
| Templates | `99_Templates/` | Standardized note creation |
| Properties | All notes | YAML frontmatter for metadata |
| Bases | `08_Metricas/` | Structured data for analytics |
| Canvas | `03_Memoria/` | Visual relationship maps |

---

## Quick Links

- [[00_Start_Here/Dashboard|Dashboard]]
- [[00_Start_Here/Quickstart_Agent|Quickstart for Agents]]
- [[01_Planejamento/Planejamento de Stack|Stack Polvo 4.1]]
- [[01_Planejamento/Planejamento de Gastos|Budget Plan]]
- [[07_Producao/Kanban|Kanban Board]]
- [[10_Changelog/Changelog|Changelog]]