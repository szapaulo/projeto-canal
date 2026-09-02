---
type: agente
status: definido
ferramentas:
  - YouTube Analytics API
  - TikTok Analytics API
  - n8n
entrada: "IDs dos vídeos publicados"
saida: "Relatório de métricas: views, retenção, watch time, CTR, likes, comentários, compartilhamentos, salvamentos, seguidores"
criado: 2026-09-02
tags: [agente, metricas]
---

# Agente: Analytics

## Função

Coletor de métricas. Após 24-72h da publicação, coleta todas as métricas disponíveis das plataformas.

---

## Responsabilidades

- Coletar views, watch time, retenção, CTR
- Coletar likes, comentários, compartilhamentos, salvamentos
- Medir crescimento de seguidores/inscritos
- Calcular velocidade de crescimento
- Popular banco de dados e notas do Obsidian

---

## Métricas Coletadas

| Métrica | YouTube | TikTok | Prioridade |
|---|---|---|---|
| Views | ✅ | ✅ | Alta |
| Watch Time | ✅ | ✅ | Alta |
| Retenção (%) | ✅ | ✅ | Alta |
| CTR | ✅ | ❌ | Média |
| Likes | ✅ | ✅ | Média |
| Comentários | ✅ | ✅ | Alta |
| Compartilhamentos | ✅ | ✅ | Alta |
| Salvamentos | ❌ | ✅ | Baixa |
| Seguidores ganhos | ✅ | ✅ | Média |

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | Trigger: 24-72h pós-publicação |
| **Input** | IDs/URLs dos vídeos |
| **Entrega para** | [[06_Agentes/Learning\|Learning]] |
| **Output** | Métricas populadas nas notas + database |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| YouTube Analytics API | Dados do YouTube |
| TikTok Analytics API | Dados do TikTok |
| n8n | Agendamento de coleta |

---

## Critérios de qualidade

- [ ] Todos os vídeos publicados têm métricas coletadas
- [ ] Dados sincronizados entre database e Obsidian