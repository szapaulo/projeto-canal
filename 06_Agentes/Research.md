---
type: agente
status: definido
ferramentas:
  - Perplexity
  - Google Trends
  - News APIs
entrada: "Tema/contexto para pesquisa"
saida: "Research brief: tema, contexto, fontes, fatos, ângulos, oportunidades, riscos"
criado: 2026-09-02
tags: [agente, discovery]
---

# Agente: Research

## Função

Pesquisador. Busca acontecimentos, tendências, notícias, fatos e fontes sobre temas selecionados.

---

## Responsabilidades

- Pesquisar acontecimentos recentes e tendências
- Levantar fatos e fontes confiáveis
- Identificar perguntas do público sobre o tema
- Mapear assuntos emergentes

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Orchestrator\|Orchestrator]] |
| **Input** | Tema ou conjunto de temas |
| **Entrega para** | [[06_Agentes/Orchestrator\|Orchestrator]], [[06_Agentes/Writer\|Writer]] |
| **Output** | Research brief estruturado |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Perplexity | Pesquisa web com fontes |
| Google Trends | Identificar tendências de busca |
| News APIs | Notícias recentes |

---

## Critérios de qualidade

- [ ] Fontes verificadas e citadas
- [ ] Fatos atualizados (últimos 7 dias)
- [ ] Pelo menos 3 ângulos identificados