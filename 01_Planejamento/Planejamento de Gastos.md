---
type: planejamento
status: definido
tags: [orcamento, stack, gastos]
---

# Polvo 4.1 — Orçamento

**Com teto rígido de R$300/mês**, a estratégia é: não tentar assinar tudo. O Polvo 4.1 precisa começar **enxuto e automatizado**.

## 🐙 POLVO 4.1 — ORÇAMENTO MÁXIMO R$300/mês

|Componente|Plano inicial|Orçamento|
|---|---|---|
|🧠 ChatGPT|seu plano atual|**R$0 adicional**|
|🧠 Claude|**Pro**|~R$100–120|
|🐙 n8n|self-hosted|**R$0**|
|🔌 MCP|open source / integrado|**R$0**|
|🧠 Obsidian|Free|**R$0**|
|🏭 MoneyPrinterTurbo|open source|**R$0**|
|🎬 CapCut|Pro|~R$66|
|🎙️ ElevenLabs|Free inicialmente|**R$0**|
|🎨 Kling|Free/créditos pontuais|**R$0 inicialmente**|
|🎥 Higgsfield|Free/créditos pontuais|**R$0 inicialmente**|
|🔎 Perplexity|Free|**R$0**|
|📊 vidIQ|Free|**R$0**|
|📈 TubeBuddy|Free|**R$0**|
|🎨 Canva|Free|**R$0**|
|🖼️ Photopea|Free|**R$0**|
|🎞️ DaVinci Resolve|Free|**R$0**|
|🐍 Python|Free|**R$0**|

O Claude Pro custa US$20/mês no pagamento mensal ou US$200/ano; ele inclui **Claude Code**, que é particularmente importante para nossa arquitetura de agentes.

O CapCut Pro aparece atualmente por **R$65,90/mês ou R$234,90/ano** na App Store brasileira, embora a própria CapCut avise que os preços podem variar por região, plataforma e promoção.

### 🎯 Resultado

**Claude Pro + CapCut Pro ≈ R$170–190/mês**, dependendo do câmbio/preço efetivamente cobrado.

Você ainda teria:

### **~R$110–130 de reserva mensal.**

E eu **não gastaria essa reserva imediatamente**.

---

# 💡 Onde colocar os R$100 restantes?

Aqui está a parte importante.

Não compre outra assinatura.

Use o dinheiro como:

### **FUNDO DE COMPUTE DO POLVO**

Para:

- créditos Kling;
- créditos Higgsfield;
- ElevenLabs;
- APIs;
- hospedagem;
- eventualmente VPS;
- modelos específicos;
- automações.

Assim você paga **pelo que o agente realmente consumir**, e não por dez assinaturas que ficam paradas.

---

# 🧠 A STACK DE R$300 FICA ASSIM

```
                    🐙 POLVO 4.1
                         │
                 ┌───────┴───────┐
                 ↓               ↓
             CHATGPT          CLAUDE PRO
                 │               │
                 │          CLAUDE CODE
                 │               │
                 └───────┬───────┘
                         ↓
                       MCP
                         ↓
                       n8n
                         ↓
              ┌──────────┼──────────┐
              ↓          ↓          ↓
          RESEARCH     VIRAL      ANALYTICS
          AGENT        AGENT       AGENT
              │          │          │
              └──────────┼──────────┘
                         ↓
                    WRITER AGENT
                         ↓
                    RED TEAM
                         ↓
                CREATIVE DIRECTOR
                         ↓
             ┌───────────┼───────────┐
             ↓           ↓           ↓
          KLING      HIGGSFIELD    IMAGEM
             │           │
             └───────────┼───────────┘
                         ↓
                    ELEVENLABS
                         ↓
                MONEYPRINTERTURBO
                         ↓
                    CAPCUT PRO
                         ↓
                       QA
                         ↓
                   PUBLICAÇÃO
                         ↓
                     MÉTRICAS
                         ↓
                  LEARNING AGENT
                         ↓
                     OBSIDIAN
                         ↓
                   NOVO CICLO
```

---

# 🚫 O QUE EU NÃO COMPRARIA AGORA

**Não assine ainda:**

- Midjourney
- Sora
- Perplexity Pro
- vidIQ Pro
- TubeBuddy Pro
- Jasper
- Copy.ai
- Nichesss
- Animoto
- InVideo
- Pictory
- Canva Pro

Isso seria **gastar dinheiro para substituir ferramentas que você já tem ou consegue usar gratuitamente**.

E tem uma razão ainda mais importante:

**MoneyPrinterTurbo + n8n + Claude Code + MCP** é justamente a combinação que permite construir sua própria infraestrutura em vez de depender de SaaS para cada etapa.

---

# 🔥 MINHA DIVISÃO DOS R$300

### R$0–190

**Infraestrutura + Claude + CapCut**

### R$0

**Memória + automação + ferramentas open source**

### R$110–300

**Créditos variáveis de produção**

Ou seja:

> **não existe obrigação de gastar os R$300 todos os meses.**

Se em determinado mês o Polvo conseguir produzir 100 vídeos gastando apenas R$210, **fica R$90 no caixa**.

Esse dinheiro pode financiar o mês seguinte.

---

## ⚠️ E UM DETALHE IMPORTANTE

Eu **não colocaria ElevenLabs pago ainda**.

O plano gratuito já serve para validar o pipeline. Depois, quando o volume de produção justificar, o primeiro upgrade provavelmente será voz ou geração de vídeo — não outra IA de texto. A lógica é simples:

**texto é barato; geração multimídia é onde o custo explode.**

Então, com **R$300/mês**, o objetivo não é ter a Stack Polvo 4.1 "completa em assinaturas".

É ter a **arquitetura completa funcionando** com o mínimo de serviços pagos.