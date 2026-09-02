---
type: agente
status: definido
ferramentas:
  - Manual review
  - Claude (análise multimodal)
entrada: "Vídeo final"
saida: "Relatório: APROVADO ou REPROVADO → agente responsável"
criado: 2026-09-02
tags: [agente, gate, producao]
---

# Agente: QA

## Função

Inspetor de qualidade. Assiste ao produto final e aprova ou rejeita antes da publicação.

---

## Checklist de Inspeção

### Conteúdo
- [ ] Precisão factual
- [ ] Coerência narrativa
- [ ] Informações corretas

### Visual
- [ ] Sem erros visíveis
- [ ] Sem artefatos de IA
- [ ] Consistência estética

### Áudio
- [ ] Volume adequado
- [ ] Sincronização voz + vídeo
- [ ] Pronúncia correta

### Retenção
- [ ] Hook forte
- [ ] Ritmo sem partes mortas
- [ ] Payoff satisfatório

---

## Decisão

| Resultado | Ação |
|---|---|
| **APROVADO** | Encaminhar para Distribution |
| **REPROVADO** | Devolver ao agente responsável com issues específicas |

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Editor\|Editor]] |
| **Input** | Vídeo final |
| **Entrega para** | [[06_Agentes/Distribution\|Distribution]] (se aprovado) |
| **Output** | Relatório QA |

---

## Critérios de qualidade

- [ ] Todos os checklists preenchidos
- [ ] Issues específicas quando reprovado