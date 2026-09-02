---
type: agente
status: definido
ferramentas:
  - Claude
  - ChatGPT
entrada: "Tema + ângulo selecionado"
saida: "10+ hooks avaliados por curiosidade, especificidade, surpresa, conflito, promessa, tensão"
criado: 2026-09-02
tags: [agente, criacao]
---

# Agente: Hook

## Função

Especialista nos primeiros segundos. Cria e avalia hooks que prendem a atenção antes do scroll.

---

## Responsabilidades

- Gerar 10+ variações de hook
- Avaliar cada hook em: curiosidade, especificidade, surpresa, conflito, promessa, tensão, lacuna de informação
- Selecionar os 3 melhores

---

## Critérios de Avaliação

| Critério | Peso | Descrição |
|---|---|---|
| Curiosidade | 25% | Gera vontade de saber mais? |
| Especificidade | 20% | É concreto ou genérico? |
| Surpresa | 20% | É inesperado? |
| Promessa | 20% | Promete valor claro? |
| Tensão | 15% | Cria urgência ou conflito? |

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Angle\|Angle]] |
| **Input** | Tema + ângulo selecionado |
| **Entrega para** | [[06_Agentes/Writer\|Writer]] |
| **Output** | Top 3 hooks com scores |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Claude/ChatGPT | Geração e avaliação de hooks |
| Obsidian | Biblioteca de hooks em `03_Memoria/Hooks/` |

---

## Critérios de qualidade

- [ ] Mínimo 10 hooks gerados
- [ ] Top 3 com score >7/10 em todos os critérios
- [ ] Hooks catalogados na memória