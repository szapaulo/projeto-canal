---
type: agente
status: definido
ferramentas:
  - TikTok API (via scraping)
  - YouTube Data API
  - GetPoppy
  - vidIQ
entrada: "Plataformas e nichos para monitorar"
saida: "Lista de conteúdos com crescimento anormal (views, velocidade, engajamento)"
criado: 2026-09-02
tags: [agente, discovery]
---

# Agente: Viral Hunter

## Função

Caçador. Monitora plataformas em busca de conteúdos com crescimento anormal — o que está **começando** a viralizar, não o que já viralizou.

---

## Responsabilidades

- Monitorar TikTok, YouTube, Instagram, Facebook
- Detectar crescimento anormal de views
- Medir velocidade de crescimento
- Analisar engajamento (comentários, compartilhamentos)
- Identificar assuntos recorrentes e formatos repetidos

---

## Pergunta-chave

> Não: "O que está viral?"
> Sim: **"O que está começando a viralizar?"**

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Orchestrator\|Orchestrator]] |
| **Input** | Plataformas, nichos, thresholds |
| **Entrega para** | [[06_Agentes/Viral Analyst\|Viral Analyst]] |
| **Output** | Lista de virais candidatos com metadados |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| TikTok | Radar de tendências |
| YouTube | Radar + vidIQ/TubeBuddy |
| GetPoppy | Inteligência de conteúdo |
| vidIQ | Métricas YouTube |

---

## Critérios de qualidade

- [ ] Conteúdos identificados ainda em ascensão (não pico já passado)
- [ ] Mínimo de 3 candidatos por rodada
- [ ] Metadados completos (views, velocidade, engajamento)