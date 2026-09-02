---
type: agente
status: definido
ferramentas:
  - Claude
  - ChatGPT
entrada: "Roteiro completo"
saida: "Relatório: APROVADO ou REPROVADO com feedback específico"
criado: 2026-09-02
tags: [agente, gate, criacao]
---

# Agente: Red Team

## Função

Crítico. Tenta matar a ideia antes do público matar. Gate obrigatório entre roteiro e produção.

---

## Checklist de Avaliação

- [ ] O hook é fraco ou genérico?
- [ ] Parece conteúdo de IA (artificial, sem alma)?
- [ ] A promessa é falsa ou exagerada?
- [ ] Existe informação desnecessária (gorda)?
- [ ] O payoff entrega o que foi prometido?
- [ ] O ritmo cai em algum ponto?
- [ ] Existe algum ponto factual vulnerável?
- [ ] O vídeo tem motivo para ser compartilhado?

---

## Decisão

| Resultado | Ação |
|---|---|
| **APROVADO** (>7/10) | Encaminhar para Creative Director |
| **REPROVADO** (≤7/10) | Devolver ao Writer com feedback específico |

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Writer\|Writer]] |
| **Input** | Roteiro completo |
| **Entrega para** | [[06_Agentes/Creative Director\|Creative Director]] (se aprovado) ou [[06_Agentes/Writer\|Writer]] (se reprovado) |
| **Output** | Relatório de avaliação + decisão |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Claude/ChatGPT | Análise crítica |

---

## Critérios de qualidade

- [ ] Todos os 8 critérios avaliados
- [ ] Feedback específico e acionável quando reprovado
- [ ] Score numérico registrado