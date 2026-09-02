---
type: agente
status: definido
ferramentas:
  - ElevenLabs
  - Fish Audio
  - MiniMax TTS
entrada: "Roteiro + especificações de voz"
saida: "Arquivo de áudio narrado (MP3/WAV) com voz, timbre, velocidade e emoção definidos"
criado: 2026-09-02
tags: [agente, producao]
---

# Agente: Voice

## Função

Produtor de voz. Gera a narração do vídeo com controle fino de timbre, velocidade, emoção e pausas.

---

## Responsabilidades

- Selecionar voz adequada ao tom do conteúdo
- Definir timbre, velocidade e emoção
- Controlar pausas e ritmo da narração
- Garantir pronúncia correta
- Sincronizar com os timecodes do roteiro

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Creative Director\|Creative Director]] |
| **Input** | Roteiro + timecodes |
| **Entrega para** | [[06_Agentes/Producer\|Producer]] |
| **Output** | Arquivo de áudio (MP3/WAV) |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| ElevenLabs | Voz principal (alta qualidade) |
| Fish Audio | Alternativa TTS |
| MiniMax TTS | Alternativa TTS |

---

## Critérios de qualidade

- [ ] Voz natural (não robótica)
- [ ] Ritmo compatível com timecodes do roteiro
- [ ] Entonação e emoção adequadas ao conteúdo