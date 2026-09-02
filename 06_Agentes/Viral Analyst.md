---
type: agente
status: definido
ferramentas:
  - Claude
  - ChatGPT
entrada: "Conteúdo viral (vídeo/script + metadados)"
saida: "DNA do viral: hook, promise, curiosity gap, development, tension, payoff, CTA + métricas de estrutura"
criado: 2026-09-02
tags: [agente, discovery]
---

# Agente: Viral Analyst

## Função

Desmontador. Recebe um conteúdo viral e o quebra em componentes atômicos para entender por que funcionou.

---

## Responsabilidades

- Desmontar estrutura narrativa: hook → promise → curiosity gap → development → tension → payoff → CTA
- Analisar: duração, ritmo, cortes, texto, áudio, estética, emoção
- Gerar o DNA do viral como modelo replicável

---

## Output (Estrutura do DNA)

```
HOOK       → O que prendeu nos primeiros 3 segundos
PROMESSA   → O que o espectador espera receber
CURIOSITY  → Lacuna de informação criada
DEVELOP    → Como a informação é entregue
TENSION    → O que mantém o interesse
PAYOFF     → A entrega final
CTA        → Call to action
```

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Viral Hunter\|Viral Hunter]] |
| **Input** | Viral + metadados |
| **Entrega para** | [[06_Agentes/Angle\|Angle]] |
| **Output** | DNA do viral documentado |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Claude/ChatGPT | Análise profunda de estrutura |
| Obsidian | Armazenar DNA em `03_Memoria/Virais/` |

---

## Critérios de qualidade

- [ ] Todos os 7 componentes do DNA identificados
- [ ] Métricas objetivas (duração, cortes, ritmo)
- [ ] DNA salvo em nota estruturada