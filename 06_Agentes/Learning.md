---
type: agente
status: definido
ferramentas:
  - Claude
  - Python (data analysis)
entrada: "Métricas reais + previsões anteriores"
saida: "Relatório de aprendizado: o que acertamos, o que erramos, o que ajustar"
criado: 2026-09-02
tags: [agente, metricas, aprendizado]
---

# Agente: Learning

## Função

Aprendiz do feedback loop. Compara previsões com resultados reais e atualiza o sistema para melhorar o próximo ciclo.

---

## Responsabilidades

- Comparar previsão de performance vs. resultado real
- Identificar onde o sistema errou e onde acertou
- Atualizar pesos de decisão dos agentes
- Registrar lições aprendidas no Obsidian

---

## Exemplo de Aprendizado

```
Hook A
Previsão: 8/10
Resultado: 4/10

Hook B
Previsão: 7/10
Resultado: 9/10

→ Aprendizado: Minha previsão sobre hooks tipo "mistério" estava superestimada.
  Hooks tipo "dinheiro" performam melhor do que o previsto.
```

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Analytics\|Analytics]] |
| **Input** | Métricas reais |
| **Entrega para** | [[06_Agentes/Pattern Miner\|Pattern Miner]], Obsidian |
| **Output** | Relatório de aprendizados + ajustes nos agentes |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Claude/ChatGPT | Análise comparativa |
| Python | Processamento de dados |
| Obsidian | Registrar em `08_Metricas/Aprendizados/` |

---

## Critérios de qualidade

- [ ] Toda publicação gera um registro de aprendizado
- [ ] Previsões comparadas com resultados em todas as métricas-chave
- [ ] Ajustes propagados para os agentes relevantes (Hook, Angle, Writer)