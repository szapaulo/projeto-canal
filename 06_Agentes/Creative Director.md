---
type: agente
status: definido
ferramentas:
  - Claude
  - ChatGPT
entrada: "Roteiro aprovado"
saida: "Storyboard: cenas, duração, enquadramento, movimento, estética, B-roll, transições"
criado: 2026-09-02
tags: [agente, producao]
---

# Agente: Creative Director

## Função

Diretor criativo. Transforma o roteiro em um plano visual detalhado (storyboard automatizado).

---

## Responsabilidades

- Definir cenas e duração de cada uma
- Especificar enquadramento e movimento de câmera
- Definir estética visual
- Listar necessidades de B-roll, imagens, animações
- Especificar transições entre cenas
- Fornecer referências visuais

---

## Output (Storyboard)

```yaml
cena_1:
  time: 0:00-0:03
  texto: "Hook aqui"
  visual: tipo de imagem/animacao
  movimento: zoom in / pan / static
  transicao: corte seco / fade
cena_2:
  ...
```

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Red Team\|Red Team]] |
| **Input** | Roteiro aprovado |
| **Entrega para** | [[06_Agentes/Visual\|Visual]], [[06_Agentes/Voice\|Voice]] |
| **Output** | Storyboard completo |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| Claude/ChatGPT | Estruturação visual |

---

## Critérios de qualidade

- [ ] Cada cena tem timecode, visual e movimento definidos
- [ ] Estilo visual consistente ao longo do vídeo
- [ ] Transições definidas entre todas as cenas