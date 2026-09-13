---
type: agente
status: definido
ferramentas:
  - Claude
  - ChatGPT
entrada: "Tema + viral DNA + research brief"
saida: "3-5 ângulos ranqueados por potencial"
criado: 2026-09-02
tags: [agente, criacao]
---

# Agente: Angle

## Função

Especialista em ângulo. Para um mesmo tema, gera múltiplas formas de abordagem e seleciona as de maior potencial.

---

## Responsabilidades

- Gerar variações de ângulo para cada tema
- Categorizar por tipo: medo, dinheiro, curiosidade, futuro, ameaça, oportunidade, controvérsia, descoberta, tutorial
- Ranquear por potencial de engajamento

---

## Exemplo

**Tema:** Inteligência Artificial

| Ângulo | Tipo | Potencial |
|---|---|---|
| "IA vai substituir seu emprego em 2027" | Medo | Alto |
| "Como ganhar dinheiro com IA sem saber programar" | Dinheiro | Alto |
| "O segredo do ChatGPT que ninguém te contou" | Curiosidade | Médio |

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Viral Analyst\|Viral Analyst]] |
| **Input** | Tema + DNA de virais similares |
| **Entrega para** | [[06_Agentes/Hook\|Hook]] |
| **Output** | Ângulos ranqueados |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Claude/ChatGPT | Geração criativa de ângulos |
| Obsidian | Consultar `03_Conhecimento_Base/07_Angulos/` |

---

## Critérios de qualidade

- [ ] Mínimo 5 ângulos por tema
- [ ] Cada ângulo classificado por tipo
- [ ] Ranking com justificativa