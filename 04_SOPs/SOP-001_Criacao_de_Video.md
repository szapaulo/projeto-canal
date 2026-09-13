---
type: sop
status: rascunho
versao: 1.0
criado: 2026-09-02
agentes:
  - Orchestrator
  - Research
  - Viral Hunter
  - Viral Analyst
  - Angle
  - Hook
  - Writer
  - Red Team
  - Creative Director
  - Visual
  - Voice
  - Producer
  - Editor
  - QA
  - Distribution
ferramentas:
  - n8n
  - MCP
  - MoneyPrinterTurbo
  - CapCut Pro
  - ElevenLabs
  - Kling/Higgsfield
---

# SOP-001: Full Video Creation — Discovery to Publishing

## Objective

Define the end-to-end autonomous flow for creating a single video, from opportunity discovery to multi-platform publishing.

## Prerequisites

- [ ] n8n self-hosted running with MCP integration
- [ ] Claude API access (via Claude Code or MCP)
- [ ] MoneyPrinterTurbo configured locally
- [ ] CapCut Pro installed
- [ ] ElevenLabs API key (free tier acceptable initially)
- [ ] Kling/Higgsfield account with credits
- [ ] YouTube + TikTok accounts created
- [ ] Obsidian vault synced

---

## Flow

### Stage 1 — Opportunity Discovery

**Agents:** [[06_Agentes/Orchestrator|Orchestrator]], [[06_Agentes/Research|Research]], [[06_Agentes/Viral Hunter|Viral Hunter]]

**Trigger:** Scheduled (daily) or manual

**Actions:**
1. Orchestrator spawns Viral Hunter to scan platforms (TikTok, YT Shorts, IG Reels) for anomalous growth
2. Viral Hunter returns list of candidate virals with metadata (views, velocity, engagement)
3. Orchestrator spawns Research Agent to gather context on top candidates (facts, sources, news)
4. Orchestrator selects the highest-potential opportunity

**Output:**
- `03_Conhecimento_Base/04_Virais_Tendencias/` — cataloged viral with metadata
- Research brief: `07_Producao/Ideias/` — new idea note created

---

### Stage 2 — Viral DNA Breakdown

**Agent:** [[06_Agentes/Viral Analyst|Viral Analyst]]

**Input:** Selected viral + research brief

**Actions:**
1. Analyze viral structure: hook → promise → curiosity gap → development → tension → payoff → CTA
2. Measure: duration, rhythm, cuts, text, audio, aesthetic, emotion, narrative structure
3. Generate DNA report

**Output:**
- DNA structure saved to viral note in `03_Conhecimento_Base/04_Virais_Tendencias/`
- Extracted patterns stored in `03_Conhecimento_Base/05_Padroes_Vencedores/` if new

---

### Stage 3 — Angle Selection

**Agent:** [[06_Agentes/Angle|Angle]]

**Input:** Theme + viral DNA

**Actions:**
1. Generate 5-10 angle variations (fear, money, curiosity, controversy, tutorial, discovery, etc.)
2. Rank by estimated potential
3. Select top 2-3 angles

**Output:**
- Angle list in idea note: `07_Producao/Ideias/`

---

### Stage 4 — Hook Generation

**Agent:** [[06_Agentes/Hook|Hook]]

**Input:** Theme + selected angle

**Actions:**
1. Generate 10+ hooks
2. Evaluate each on: curiosity, specificity, surprise, conflict, promise, tension, information gap
3. Select top 3 hooks

**Output:**
- Hook list in idea note
- Hooks cataloged in `03_Conhecimento_Base/03_Formatos_Hooks/Hooks/`

---

### Stage 5 — Script Writing

**Agent:** [[06_Agentes/Writer|Writer]]

**Input:** Theme + angle + hook + viral DNA + research

**Actions:**
1. Generate full script with: hook, promise, curiosity gap, development, tension, payoff, CTA
2. Format as time-coded script (seconds per section)

**Output:**
- Full script saved to `07_Producao/Roteiros/`

---

### Stage 6 — Red Team Review ⚠️ GATE

**Agent:** [[06_Agentes/Red Team|Red Team]]

**Input:** Complete script + viral DNA

**Actions:**
1. Try to kill the idea before the audience does:
   - Hook weak? Generic? Sounds like AI? False promise?
   - Unnecessary info? Payoff fails? Rhythm drops?
   - Factually vulnerable? Share-worthy?

**Decision:**
- **APPROVED** → proceed to Stage 7
- **REJECTED** → return to Stage 5 (Writer) with specific feedback

**Output:**
- Red Team report with score and specific notes

---

### Stage 7 — Creative Direction (Storyboard)

**Agent:** [[06_Agentes/Creative Director|Creative Director]]

**Input:** Approved script

**Actions:**
1. Define: scenes, duration per scene, framing, movement, aesthetic
2. Specify: B-roll needs, image types, animations, transitions
3. Provide visual references

**Output:**
- Storyboard document in video note `07_Producao/Videos/`

---

### Stage 8 — Visual + Voice Production (Parallel)

**Agents:** [[06_Agentes/Visual|Visual]], [[06_Agentes/Voice|Voice]]

**Input:** Storyboard

**Actions (Visual):**
1. Generate images via Midjourney/ChatGPT Image/Canva
2. Generate video clips via Kling/Higgsfield
3. Collect B-roll material

**Actions (Voice):**
1. Generate narration via ElevenLabs
2. Define: voice, timbre, speed, emotion, pauses, pronunciation
3. Export audio file

**Output:**
- Media assets folder
- Audio file (MP3/WAV)

---

### Stage 9 — Video Assembly

**Agent:** [[06_Agentes/Producer|Producer]]

**Input:** Script + media assets + audio

**Actions:**
1. Feed into MoneyPrinterTurbo
2. Assemble: script → media → voice → subtitles → music → video

**Output:**
- Raw video file (MP4)

---

### Stage 10 — Editing

**Agent:** [[06_Agentes/Editor|Editor]]

**Input:** Raw video

**Actions:**
1. Import into CapCut Pro
2. Enhance: rhythm, cuts, subtitles, zoom, B-roll, music, effects, transitions
3. Export final video

**Output:**
- Final video file (MP4)

---

### Stage 11 — QA Review ⚠️ GATE

**Agent:** [[06_Agentes/QA|QA]]

**Input:** Final video

**Checks:**
- **Content:** accuracy, coherence, narrative
- **Visual:** errors, artifacts, inconsistencies
- **Audio:** volume, sync, pronunciation
- **Retention:** hook strength, rhythm, dead spots

**Decision:**
- **APPROVED** → proceed to Stage 12
- **REJECTED** → return to responsible agent with specific issues

**Output:**
- QA report with score

---

### Stage 12 — Distribution

**Agent:** [[06_Agentes/Distribution|Distribution]]

**Input:** Approved video + metadata

**Actions:**
1. Adapt for each platform: TikTok, YouTube Shorts, IG Reels, FB Reels
2. Generate: title, description, hashtags, CTA, thumbnail (if needed), variations
3. Schedule or publish

**Output:**
- Video published on target platforms
- `07_Producao/Publicados/` — published note created
- Status updated: `status: publicado`

---

### Stage 13 — Wait & Collect

**Timing:** 24-72 hours after publication

---

### Stage 14 — Analytics Collection

**Agent:** [[06_Agentes/Analytics|Analytics]]

**Input:** Published video IDs

**Actions:**
1. Collect: views, retention, watch time, CTR, likes, comments, shares, saves, followers
2. Populate video note with metrics

**Output:**
- Metrics in `07_Producao/Publicados/` and `08_Metricas/`

---

### Stage 15 — Learning & Pattern Mining

**Agents:** [[06_Agentes/Learning|Learning]], [[06_Agentes/Pattern Miner|Pattern Miner]]

**Input:** Published metrics + predictions

**Actions:**
1. Compare prediction vs. real result
2. Update memory: which hooks/angles/formats work
3. Pattern Miner searches for correlations across all published content

**Output:**
- Updated `03_Conhecimento_Base/05_Padroes_Vencedores/`
- Updated agent prediction weights
- Memory stored in Obsidian

---

## Error Handling

| Error | Cause | Action |
|---|---|---|
| Agent fails to respond | API timeout, quota | Retry 3x with exponential backoff; escalate to Orchestrator |
| MoneyPrinterTurbo fails | Missing media, config error | Log error; manual intervention if 3 retries fail |
| Video generation fails | API credits exhausted | Use free tier alternative; log budget consumption |
| QA rejects 3+ times | Systemic issue in pipeline | Escalate to Orchestrator; pause pipeline for review |
| Publishing fails | API rate limit, auth error | Retry with different schedule; verify credentials |

---

## Expected Output

One short-form video (~30-60s) published across 2+ platforms, with full traceability from discovery to metrics.

## Changelog

| Version | Date | Change |
|---|---|---|
| 1.0 | 2026-09-02 | Initial SOP created during vault restructuring |