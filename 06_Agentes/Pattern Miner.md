---
type: agente
status: definido
ferramentas:
  - Claude
  - Python (data mining)
  - Database (SQL)
entrada: "Milhares de conteúdos publicados + métricas"
saida: "Padrões vencedores: combinações de hook + duração + tema + payoff + visual + CTA com maior performance"
criado: 2026-09-02
tags: [agente, metricas, aprendizado]
---

# Agente: Pattern Miner

## Função

Minerador de padrões. Cruza milhares de dados para encontrar combinações vencedoras recorrentes.

---

## Responsabilidades

- Procurar correlações entre elementos e performance
- Identificar padrões de hooks vencedores
- Identificar durações ideais por formato/plataforma
- Gerar conhecimento proprietário do Polvo

---

## Exemplo de Padrão Descoberto

```yaml
padrao: "Mistério + Dinheiro"
hook: "Você provavelmente não sabe..."
duracao: 24-31s
tema: mistério + oportunidade financeira
payoff: últimos 20% do vídeo
visual: cortes rápidos, imagens impactantes
cta: pergunta aberta nos comentários
performance:
  views_medio: 2.3M
  retencao_media: 73%
  engajamento: alto
```

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Learning\|Learning]] + Database |
| **Input** | Todos os dados históricos |
| **Entrega para** | Obsidian (`03_Memoria/Padroes_Vencedores/`) + Orchestrator |
| **Output** | Padrões ranqueados por performance |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Python | Mineração de dados, estatística |
| Database (SQL) | Queries em dados quantitativos |
| Claude | Interpretação de padrões, geração de insights |
| Obsidian | Armazenar padrões como conhecimento proprietário |

---

## Critérios de qualidade

- [ ] Padrões baseados em dados reais (mínimo 10 amostras)
- [ ] Significância estatística verificada
- [ ] Padrões alimentam os agentes Angle, Hook e Writer