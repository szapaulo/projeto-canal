---
type: agente
status: definido
ferramentas:
  - MoneyPrinterTurbo
entrada: "Roteiro + assets visuais + áudio"
saida: "Vídeo-base montado (MP4)"
criado: 2026-09-02
tags: [agente, producao]
---

# Agente: Producer

## Função

Linha de montagem. Recebe todos os assets e monta o vídeo-base via MoneyPrinterTurbo.

---

## Pipeline de Montagem

```
ROTEIRO → MÍDIA → VOZ → LEGENDA → MÚSICA → MONTAGEM → VÍDEO-BASE
```

---

## Responsabilidades

- Alimentar MoneyPrinterTurbo com roteiro + mídia + voz
- Configurar parâmetros de montagem
- Gerar vídeo-base (primeira versão antes da edição fina)

---

## Input / Output

| Direção | Descrição |
|---|---|
| **Recebe de** | [[06_Agentes/Visual\|Visual]], [[06_Agentes/Voice\|Voice]] |
| **Input** | Roteiro + assets visuais + áudio |
| **Entrega para** | [[06_Agentes/Editor\|Editor]] |
| **Output** | Vídeo-base MP4 |

---

## Ferramentas

| Ferramenta | Propósito |
|---|---|
| MoneyPrinterTurbo | Automação completa de montagem de vídeo |

---

## Critérios de qualidade

- [ ] Vídeo renderizado sem erros
- [ ] Sincronização básica áudio + vídeo
- [ ] Legendas geradas corretamente