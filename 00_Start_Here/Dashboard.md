# Dashboard — Polvo 4.1

> Última atualização: `$= dv.current().file.mtime`

---

## 🎯 Status Geral

| Indicador                  | Valor                                                                                   |     |                       |     |                                |
| -------------------------- | --------------------------------------------------------------------------------------- | --- | --------------------- | --- | ------------------------------ |
| Fase atual                 | Estudo & Planejamento                                                                   |     |                       |     |                                |
| Orçamento mensal           | R$300                                                                                   |     |                       |     |                                |
| Gastos este mês            | `$= dv.pages('"01_Planejamento"').where(p => p.type == "gasto").sum(p => p.valor) ?? 0` |     |                       |     |                                |
| Vídeos em produção         | `$= dv.pages('"07_Producao"').where(p => p.status == "em_producao"                      |     | p.status == "roteiro" |     | p.status == "revisao").length` |
| Vídeos publicados este mês | `$= dv.pages('"07_Producao"').where(p => p.status == "publicado").length`               |     |                       |     |                                |

---

## 📋 Produção Ativa

```dataview
TABLE WITHOUT ID
  file.link AS "Vídeo",
  tema AS "Tema",
  formato AS "Formato",
  status AS "Status",
  deadline AS "Prazo"
FROM "07_Producao"
WHERE type = "video" AND status != "publicado" AND status != "arquivado"
SORT priority ASC, deadline ASC
```

---

## ✅ Últimos Publicados

```dataview
TABLE WITHOUT ID
  file.link AS "Vídeo",
  plataforma AS "Plataforma",
  publicado_em AS "Data",
  views AS "Views"
FROM "07_Producao"
WHERE type = "video" AND status = "publicado"
SORT publicado_em DESC
LIMIT 10
```

---

## 📚 Estudos em Andamento

```dataview
TABLE WITHOUT ID
  file.link AS "Tópico",
  categoria AS "Categoria",
  nivel AS "Nível"
FROM "02_Estudo"
WHERE type = "estudo" AND status = "em_andamento"
SORT nivel DESC
```

---

## 📝 Estudos Pendentes

```dataview
TABLE WITHOUT ID
  file.link AS "Tópico",
  categoria AS "Categoria"
FROM "02_Estudo"
WHERE type = "estudo" AND status = "pendente"
SORT file.name ASC
LIMIT 10
```

---

## 🔬 Experimentos Ativos

```dataview
TABLE WITHOUT ID
  file.link AS "Experimento",
  status AS "Status",
  resultado AS "Resultado"
FROM "03_Memoria/Experimentos"
WHERE type = "experimento"
SORT file.mtime DESC
```

---

## 🔗 Links Rápidos

- [[07_Producao/Kanban|Quadro Kanban]]
- [[01_Planejamento/Planejamento de Stack|Stack Polvo 4.1]]
- [[01_Planejamento/Planejamento de Gastos|Orçamento]]
- [[10_Changelog/Changelog|Histórico de Mudanças]]
- [[02_Estudo/00_Estudo|MOC de Estudos]]
- [[04_SOPs/SOPs|Procedimentos Operacionais]]