---
type: moc
tags: [taxonomia, moc]
atualizado: 2026-09-09
---

# Taxonomia — 03_Conhecimento_Base

Estrutura conceitual do projeto: **Áreas > Temas > Nichos**

---

## Visão Geral

A taxonomia é a espinha dorsal do sistema Polvo 4.1. Ela permite:
- Organizar ideias de forma hierárquica
- Definir o escopo de cada nicho
- Facilitar a descoberta de conteúdo relacionado
- Apoiar decisões estratégicas sobre monetização
- Garantir que não descubramos as mesmas coisas duas vezes

---

## Hierarquia Completa

```
03_Conhecimento_Base/
├── 02_Taxonomia/
│   ├── 00_Mestre.md              # Esta nota (Map of Content da taxonomia)
│   ├── Areas.md                  # Macro-categorias e matriz de seleção
│   ├── Temas.md                  # Lista geral de temas organizados por área
│   ├── Nichos.md                 # Lista geral de nichos com critérios
│   ├── Areas/                    # Detalhamento de cada área
│   │   ├── Entretenimento.md
│   │   ├── Educacao.md
│   │   ├── Tecnologia.md
│   │   ├── Criatividade.md
│   │   └── Saude.md
│   ├── Temas/                    # Detalhamento de cada tema
│   │   ├── Arte.md
│   │   ├── Criatividade.md
│   │   ├── Curiosidades.md
│   │   ├── Educacao.md
│   │   ├── Saude.md
│   │   ├── Tecnologia.md
│   │   └── [outros_temas].md
│   └── Nichos/                   # Detalhamento de cada nicho
│       ├── Games.md
│       └── [outros_nichos].md
```

---

## Definições

| Nível | O que é | Exemplo | Função | Dados para validação |
|---|---|---|---|---|
| **Área** | Macro-categoria que agrupa temas relacionados | Entretenimento, Educação, Saúde | Define escopo geral do conteúdo | Tamanho do mercado, tendências globais |
| **Tema** | Assunto específico dentro de uma área | IA, Dota 2, Física, Breakdance | Gera conteúdo específico | Volume de buscas, crescimento YoY |
| **Nicho** | Segmento comercial com público definido | Gamers casuais, estudantes de ENEM | Define público-alvo para monetização | CPM, taxa de engajamento, LTV |

### Regras de Classificação

1. **Um Tema pertence a uma única Área** (pode ter ligações cruzadas temáticas, mas classificação primária única)
2. **Um Nicho pode conter múltiplos Temas** (ex: nicho "Gamers casuais" pode abordar temas de Games, Tecnologia e Criatividade)
3. **Áreas são fixas no início do projeto**, mas podem ser expandidas com validação de dados
4. **Temas podem evoluir** com base em tendências emergentes
5. **Nichos são validados com dados reais** de engajamento e monetização antes de serem considerados "ativos"
6. **Sempre atualizar esta nota** quando adicionar nova área, tema ou nicho

---

## Framework de Decisão

### Etapa 1: Seleção de Áreas
Use a matriz em [[03_Conhecimento_Base/02_Taxonomia/Areas\|Areas.md]] para avaliar:
- Potencial de engajamento (0-10)
- Potencial de monetização (0-10)
- Nível de concorrência (0-10, invertido para scoring)
- Esforço de produção (0-10, invertido)
- Alinhamento com habilidades da equipe (0-10)
- **Score final** = soma ponderada

### Etapa 2: Definição de Temas
Para cada área selecionada:
- Liste todos os temas relevantes
- Avalie cada tema por:
  - Relevância para a área
  - Volume de busca mensal
  - Crescimento de interesse (Google Trends)
  - Potencial de combinação com outros temas
  - Facilidade de produção de conteúdo
- Selecione 3-5 temas prioritários por área

### Etapa 3: Validação de Nichos
Para cada tema selecionado:
- Identifique 1-3 nichos possíveis
- Valide cada nicho com:
  - Tamanho do público-alvo (inscritos em canais similares)
  - Taxa de engajamento média (likes/views, comentarios/views)
  - CPM estimado para o nicho
  - Facilidade de produção de conteúdo recorrente
  - Sustentabilidade a longo prazo (tendência > 6 meses)
- Apenas nichos com score > 7/10 avançam para teste

---

## Áreas Definidas (Critério: Score > 6.0 na matriz)

| Área | Score | Status | Temas Prioritários |
|---|---|---|---|
| Entretenimento | 8.2 | Em avaliação | Games, Curiosidades, Filmes/Séries |
| Criatividade | 7.5 | Em avaliação | Arte, Stop motion, Desenho, Ilusão de ótica |
| Tecnologia | 6.8 | Em avaliação | IA, Carros elétricos, Drones, Impressão 3D |
| Educação | 6.5 | Em avaliação | Ciências, Matemática, História, Eletrônica |
| Saúde | 6.2 | Em avaliação | Nutrição, Exercício, Sono, Saúde mental |

---

## Critérios para Definir Áreas

- **Engajamento potencial** (30%): Capacidade de gerar views, likes, comentários
- **Monetização** (25%): Potencial de CPM, afiliados, produtos digitais
- **Baixa concorrência** (20%): Espaço para diferenciar (score invertido)
- **Esforço de produção** (15%): Viabilidade de conteúdo consistente
- **Alinhamento equipe** (10%): Match com habilidades de Paulo e Estevão

---

## Critérios para Definir Temas

- Relevância direta para a área selecionada
- Volume de busca mensal > 50k (Brasil)
- Crescimento de interesse > 15% YoY (Google Trends)
- Potencial de gerar pelo menos 5 ângulos distintos
- Compatibilidade com formato dark (sem necessidade de aparecimento)

---

## Critérios para Validar Nichos

- **Tamanho do público**: > 100k inscritos em canais similares no Brasil
- **Engajamento**: Taxa de engajamento > 8% (likes+comentários)/views
- **Monetização**: CPM estimado > R$15 (YouTube Brasil)
- **Produção**: Possibilidade de criar 2+ vídeos/semana com recursos disponíveis
- **Sustentabilidade**: Tendência de crescimento estável ou crescente há > 6 meses
- **Diferencial**: Possibilidade de abordagem única não saturada

---

## Nichos Definidos (Validados com dados)

| Nicho | Área | Tema | Status | Score de Validação |
|---|---|---|---|---|
| [[03_Conhecimento_Base/02_Taxonomia/Nichos/Games|Games]] | Entretenimento | Games | ativo | 7.8/10 |

---

## Nichos em Avaliação (Critério: Score 5.0-7.7)

| Nicho em avaliação | Área | Tema | Score | Próximos passos |
|---|---|---|---|---|
| Estudantes de ENEM | Educação | Ciências/Matemática | 6.2 | Coletar dados de canais educacionais |
| Entusiastas de IA | Tecnologia | IA | 6.8 | Analisar CPM e engajamento em nicho de IA |
| Artistas Digitais | Criatividade | Arte/Desenho | 5.9 | Validar potencial de monetização |

---

## Links Rápidos

- [[03_Conhecimento_Base/02_Taxonomia/Areas|Áreas e matriz de seleção]]
- [[03_Conhecimento_Base/02_Taxonomia/Temas/Temas|Temas por área]]
- [[03_Conhecimento_Base/02_Taxonomia/Nichos|Nichos e critérios de validação]]