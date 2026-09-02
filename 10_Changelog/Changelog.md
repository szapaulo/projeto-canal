---
type: moc
status: ativo
tags: [changelog]
---

# Changelog

Histórico completo de decisões, mudanças e evolução do projeto Polvo 4.1.

---

## Como usar

Cada entrada deve ser um arquivo separado em `10_Changelog/` seguindo o template [[99_Templates/t-changelog|t-changelog]].

Formato de nome: `YYYY-MM-DD_Descricao_Curta.md`

---

## Linha do Tempo

```dataview
TABLE WITHOUT ID
  file.link AS "Data",
  tipo AS "Tipo",
  autor AS "Autor"
FROM "10_Changelog"
WHERE type = "changelog"
SORT file.name DESC
```

---

## Últimas Entradas

| Data | Descrição | Tipo |
|---|---|---|
| [[10_Changelog/2026-09-02_Estruturacao_Inicial|2026-09-02]] | Estruturação inicial do vault + Stack Polvo 4.1 | infraestrutura |