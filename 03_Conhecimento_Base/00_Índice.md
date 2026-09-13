---
type: moc
tags: [conhecimento_base, moc]
atualizado: 2026-09-09
---

# 03_Conhecimento_Base

Centro de inteligência acumulado pelo Polvo 4.1. Tudo que o sistema aprende sobre o que funciona e o que não funciona fica registrado aqui.

> **Regra de ouro:** O Polvo não deve descobrir as mesmas coisas duas vezes.

---

## Visão Geral

Este diretório é a **memória persistente** do sistema Polvo 4.1. Ele armazena:
- Ideias em captura e avaliação
- Taxonomia de áreas, temas e nichos
- Formatos de vídeo e hooks testados
- Conteúdos virais e tendências emergentes
- Padrões vencedores identificados por dados
- Resultados de experimentos A/B
- Ângulos de abordagem para cada tema
- Decisões estratégicas do projeto

---

## Hierarquia de Organização

```
03_Conhecimento_Base/
├── 00_Índice.md                  # Esta nota (Map of Content)
├── 01_Ideias/                    # Captura e avaliação de ideias
├── 02_Taxonomia/                 # Áreas > Temas > Nichos
├── 03_Formatos_Hooks/            # Elementos de conteúdo
├── 04_Virais_Tendencias/         # Monitoramento de tendências
├── 05_Padroes_Vencedores/        # Padrões identificados por dados
├── 06_Experimentos/              # Testes A/B e validações
├── 07_Angulos/                   # Ângulos de abordagem
└── 08_Estrategia/                # Decisões estratégicas
```

---

## Índice

| Seção | Descrição | Link |
|---|---|---|
| Ideias | Captura, comparação e avaliação de ideias | [[03_Conhecimento_Base/01_Ideias/Ideias\|Ideias]] |
| Taxonomia | Estrutura conceitual: Áreas > Temas > Nichos | [[03_Conhecimento_Base/02_Taxonomia/00_Mestre\|Taxonomia]] |
| Formatos | Catálogo de formatos de vídeo | [[03_Conhecimento_Base/03_Formatos_Hooks/Formatos/Formatos\|Formatos]] |
| Hooks | Biblioteca de hooks testados | [[03_Conhecimento_Base/03_Formatos_Hooks/Hooks\|Hooks]] |
| Virais | Conteúdos virais e tendências | [[03_Conhecimento_Base/04_Virais_Tendencias\|Virais & Tendências]] |
| Padrões | Combinações de elementos que performam | [[03_Conhecimento_Base/05_Padroes_Vencedores\|Padrões Vencedores]] |
| Experimentos | Testes A/B e resultados | [[03_Conhecimento_Base/06_Experimentos\|Experimentos]] |
| Ângulos | Ângulos de abordagem por tema | [[03_Conhecimento_Base/07_Angulos\|Ângulos]] |
| Estratégia | Decisões e planejamento | [[03_Conhecimento_Base/08_Estrategia\|Estratégia]] |

---

## Fluxo do Sistema

```
Ideias → Taxonomia → Formatos/Hooks → Virais → Padrões → Experimentos → Ângulos → Estratégia → Ação → Feedback ↺
```

**Cada ciclo fecha o circuito:** dados de performance alimentam novas decisões.

---

## Como Usar

### Fluxo de Trabalho Principal

1. **Viral Hunter** encontra conteúdo → catalogado em `04_Virais_Tendencias/`
2. **Viral Analyst** desmonta o viral → DNA registrado em `04_Virais_Tendencias/`
3. **Pattern Miner** cruza dados → padrões salvos em `05_Padroes_Vencedores/`
4. **Learning Agent** atualiza o que funciona → status alterado conforme métricas
5. **Angle Agent** define ângulos → salvos em `07_Angulos/`
6. **Hook Agent** cria hooks → salvos em `03_Formatos_Hooks/Hooks/`

### Regras de Manutenção

- **Nada é deletado:** conteúdos obsoletos recebem `status: arquivado`
- **Todo conteúdo deve ter frontmatter** com `type`, `status` e `tags`
- **Links devem usar formato wikilink** `[[path|display]]`
- **Atualizar esta nota** quando adicionar nova seção ou arquivo

---

## Critérios de Qualidade

| Critério | Padrão |
|---|---|
| Frontmatter | Obrigatório em todas as notas |
| Wikilinks | Usar `[[caminho/nota\|exibição]]` |
| Atualização | Revisar pelo menos uma vez por semana |
| Status | Usar `ativo`, `em_definicao`, `arquivado` |