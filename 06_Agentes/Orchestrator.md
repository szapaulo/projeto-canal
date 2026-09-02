---
type: agente
status: definido
ferramentas:
  - Claude
  - ChatGPT
  - n8n
  - MCP
entrada: "Objetivo de alto nível (ex: 'Encontre oportunidades no nicho X e produza as melhores')"
saida: "Pipeline executado com vídeo publicado e métricas coletadas"
criado: 2026-09-02
tags: [agente, core]
---

# Agente: Orchestrator

## Função

CEO do Polvo. Recebe o objetivo macro e decide quais agentes chamar, em qual ordem e quando repetir/rejeitar/solicitar intervenção humana.

---

## Responsabilidades

- Orquestrar o fluxo completo do pipeline
- Decidir quais agentes acionar e em qual ordem
- Avaliar outputs e decidir se repete, rejeita ou aprova
- Gerenciar gates (Red Team, QA)
- Solicitar intervenção humana quando necessário

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | Usuário / Trigger agendado no n8n |
| **Input** | Objetivo macro (nicho, formato, volume) |
| **Entrega para** | Todos os agentes |
| **Output** | Vídeo publicado + métricas + aprendizado registrado |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| n8n | Execução de workflows, triggers, filas |
| MCP | Comunicação com agentes e ferramentas externas |
| Claude/ChatGPT | Tomada de decisão estratégica |
| Obsidian | Leitura/escrita da memória do sistema |

---

## Critérios de qualidade

- [ ] Nenhum gate ignorado (Red Team, QA)
- [ ] Decisões registradas no Obsidian
- [ ] Erros tratados com retry ou escalação