---
type: moc
tags: [prompts]
---

# MOC — Prompts

Biblioteca versionada de prompts utilizados pelos agentes do Polvo.

Cada prompt é catalogado com:
- Versão (incrementada a cada melhoria)
- Modelo recomendado
- Agente que o utiliza
- Exemplo de saída esperada

---

## Catálogo por Agente

| Agente | Prompts |
|---|---|
| Research | [[05_Prompts/Pesquisa/|Pesquisa]] |
| Viral Hunter | |
| Viral Analyst | |
| Angle | |
| Hook | [[05_Prompts/Hook/|Hook]] |
| Writer | [[05_Prompts/Roteiro/|Roteiro]] |
| Red Team | |
| Creative Director | [[05_Prompts/Visual/|Visual]] |
| Visual | [[05_Prompts/Visual/|Visual]] |
| Voice | [[05_Prompts/Voz/|Voz]] |
| Distribution | |

---

## Template

[[99_Templates/t-prompt|t-prompt]]

## Versionamento

```
versao: MAJOR.MINOR
```

- `MAJOR`: mudança na estrutura/lógica do prompt
- `MINOR`: ajuste de wording, parâmetros, exemplos

Prompts antigos não são deletados — recebem `status: depreciado`.