---
type: agente
status: definido
ferramentas:
  - YouTube API
  - TikTok API
  - n8n (scheduling)
entrada: "Vídeo aprovado + metadados"
saida: "Vídeo publicado em todas plataformas-alvo com título, descrição, hashtags, thumbnail"
criado: 2026-09-02
tags: [agente, publicacao]
---

# Agente: Distribution

## Função

Distribuidor multi-plataforma. Adapta e publica o vídeo em todas as plataformas-alvo.

---

## Responsabilidades

- Adaptar vídeo para cada plataforma (aspect ratio, duração)
- Gerar título otimizado por plataforma
- Escrever descrição com hashtags
- Criar thumbnail quando necessário (YouTube)
- Gerar variações de CTA por plataforma
- Agendar ou publicar imediatamente

---

## Plataformas

| Plataforma | Formato | Thumbnail | Hashtags |
|---|---|---|---|
| YouTube Shorts | 9:16, <60s | Sim | 3-5 |
| TikTok | 9:16, <3min | Capa | 3-5 |
| Instagram Reels | 9:16, <90s | Capa | 5-10 |
| Facebook Reels | 9:16, <60s | Capa | 3-5 |

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/QA\|QA]] |
| **Input** | Vídeo final + metadados |
| **Entrega para** | [[06_Agentes/Analytics\|Analytics]] (após coleta) |
| **Output** | URLs publicadas + status |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| YouTube API | Upload programático |
| TikTok API | Upload programático |
| n8n | Agendamento e retry |

---

## Critérios de qualidade

- [ ] Publicado em pelo menos 2 plataformas
- [ ] Título e descrição únicos por plataforma
- [ ] Hashtags relevantes e não genéricas