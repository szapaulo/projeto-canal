---
type: changelog
data: 2026-09-02
autor: Claude (via opencode)
tags: [infraestrutura, estrutura]
tipo: infraestrutura
---

# 2026-09-02 — Estruturação Inicial do Vault

## Contexto

O repositório foi criado como vault Obsidian para servir de "cérebro central" do projeto Polvo 4.1 — um sistema autônomo de criação de conteúdo para canais dark usando agentes de IA.

---

## O que mudou

### Infraestrutura
- `.gitignore` criado para proteger arquivos de workspace e cache
- `.opencode/config.json` criado com contexto, regras e token budget para agentes de IA
- `README.md` reescrito em inglês como porta de entrada para agentes
- Estrutura de diretórios reorganizada de 2 pastas para 12 seções alinhadas à arquitetura Polvo 4.1

### Documentação
- 18 definições de agentes criadas em `06_Agentes/`
- SOP-001 (criação completa de vídeo) criada em `04_SOPs/`
- Glossário preenchido com ~20 termos do ecossistema de criação de conteúdo
- Templates Obsidian (7 tipos) criados em `99_Templates/`
- Dashboard com queries Dataview criado em `00_Start_Here/`
- Kanban de produção criado em `07_Producao/`
- Quickstart para agentes de IA criado em `00_Start_Here/`

### Frontmatter
- Todas as notas existentes receberam frontmatter YAML padronizado
- Wikilinks atualizados para refletir a nova estrutura de diretórios

### Stack
- Stack Polvo 4.1 consolidada como arquitetura oficial
- Orçamento definido: R$300/mês (Claude Pro + CapCut Pro = ~R$170-190, resto = fundo de compute)

---

## Impacto

- **Agentes de IA** agora têm contexto suficiente para operar neste repositório lendo apenas README + Quickstart (~800 tokens)
- **Dataview** pode indexar notas por tipo, status e tags
- **Graph View** pode agrupar notas por tipo (ideia, video, estudo, agente, etc.)
- **Kanban** pronto para receber o primeiro card de produção

---

## Próximos passos

- [ ] Criar contas no YouTube e TikTok
- [ ] Definir nicho + formato final
- [ ] Instalar e configurar MoneyPrinterTurbo
- [ ] Subir n8n self-hosted
- [ ] Preencher estudos das ferramentas (notas vazias em `02_Estudo/Ferramentas/`)
- [ ] Criar primeiros prompts em `05_Prompts/`
- [ ] Produzir primeiro vídeo de teste

---

## Arquivos alterados

- `README.md` — reescrito completamente (EN)
- `.gitignore` — criado
- `.opencode/config.json` — criado
- `00_Start_Here/Dashboard.md` — criado
- `00_Start_Here/Quickstart_Agent.md` — criado
- `01_Planejamento/*` — frontmatter adicionado, wikilinks atualizados
- `02_Estudo/*` — reorganizado, frontmatter, wikilinks atualizados
- `03_Memoria/*` — reorganizado, frontmatter adicionado
- `04_SOPs/*` — criado (SOP-001)
- `05_Prompts/Prompts.md` — criado
- `06_Agentes/*` — 18 agentes + MOC criados
- `07_Producao/*` — reorganizado, Kanban criado
- `08_Metricas/Metricas.md` — criado
- `09_Automacoes/Automacoes.md` — atualizado
- `10_Changelog/*` — criado (esta entrada)
- `99_Templates/*` — 8 templates criados
- `.obsidian/` — sem alterações (plugins mantidos)