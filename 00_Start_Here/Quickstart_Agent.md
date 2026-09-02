# Quickstart for AI Agents

You are operating in the **Polvo 4.1 Central Brain** — an Obsidian vault that serves as the memory and planning center for an autonomous dark-channel content creation system.

## Entry Protocol

```yaml
step_1: Read README.md (this file's parent) — mission, architecture, budget, rules
step_2: Read 10_Changelog/Changelog.md (last 3 entries) — recent decisions
step_3: Identify task type and read only relevant files (see table below)
step_4: Execute task, log changes in Changelog
```

## Task-to-File Mapping

| Task | Read These | Skip |
|---|---|---|
| Define strategy/niche | `01_Planejamento/*`, `03_Memoria/Nichos/*`, `03_Memoria/Temas/*` | Production files |
| Research a tool | `02_Estudo/Ferramentas/*` | Everything else |
| Create a video | `04_SOPs/SOP-001_*`, `05_Prompts/Roteiro/*`, `07_Producao/*` | Study files |
| Build an agent | `06_Agentes/*`, `01_Planejamento/Planejamento de Stack.md` | Production files |
| Analyze metrics | `08_Metricas/*`, `03_Memoria/Padroes_Vencedores/*` | Study files |
| Build automation | `09_Automacoes/*`, `04_SOPs/*` | Content files |
| Update project status | `00_Start_Here/Dashboard.md`, `07_Producao/Kanban.md` | — |
| General research | `02_Estudo/*`, `01_Planejamento/Glossario.md` | Production files |

## Conventions

- **Technical files** (this file, README, .opencode, SOPs, scripts, agent definitions): **English**
- **Planning/study/content notes**: **Portuguese (pt-BR)**
- **Frontmatter keys**: always in English
- **Wikilinks**: use `[[folder/note|display name]]` format
- **Frontmatter `type` field** determines note category: `ideia`, `video`, `estudo`, `sop`, `prompt`, `agente`, `changelog`, `moc`

## Frontmatter Standards

Every note must have a `type` property. Other fields depend on type:

### type: ideia
```yaml
type: ideia
status: [backlog, em_pesquisa, em_producao, publicado, arquivado]
tema: string
formato: string
nicho: string
plataforma: [list]
prioridade: [1-5]
criado: date
```

### type: video
```yaml
type: video
status: [roteiro, producao, revisao, aprovado, publicado]
ideia: "[[wikilink]]"
tema: string
formato: string
plataforma: [list]
publicado_em: date
views: number
```

### type: estudo
```yaml
type: estudo
categoria: [ferramenta, conceito, plataforma, algoritmo, formato]
status: [pendente, em_andamento, concluido]
nivel: [1-5]
```

### type: agente
```yaml
type: agente
status: [definido, em_desenvolvimento, ativo]
ferramentas: [list]
entrada: string
saida: string
```

## Critical Rules

1. **R$300/month budget ceiling** — never propose costs exceeding this
2. **Log ALL decisions** in `10_Changelog/Changelog.md`
3. **Never delete** files from `03_Memoria/` — archive with `status: arquivado` instead
4. **Prompt versioning** — when modifying prompts, increment version in frontmatter
5. **No copyrighted content** — original or properly licensed only

## Before Making Changes

- Check if a relevant SOP exists in `04_SOPs/`
- Check if a template exists in `99_Templates/`
- Review recent changelog entries for context
- Confirm budget impact if any paid service is involved