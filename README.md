# mat-saude-digital-taxonomia

**Versão:** v1.0 — 2026-05-22
**Tipo:** M02 — Matriz
**Mantenedor:** victorarimatea
**Visibilidade:** Público
**Status:** Ativo

---

## O que é esta taxonomia

A taxonomia de saúde digital é um **mapa de navegação temática** — uma estrutura
hierárquica de Partes, capítulos e subtópicos que organiza o território do
conhecimento em saúde digital. Ela não define termos: **classifica assuntos**.

Pense nela como o índice de uma enciclopédia técnica de saúde digital. Cada
entrada é um endereço — não uma explicação.

---

## Distinção essencial: Taxonomia vs. Glossário

Este repositório (M02) e o `GLOSSARIO.md` do hub-fonte (M01) são instrumentos
complementares com propósitos distintos. Entender a diferença é fundamental
para usar o ecossistema corretamente.

| | Taxonomia (M02) | Glossário (M01) |
|---|---|---|
| **Pergunta que responde** | *Onde este assunto está no mapa?* | *O que este termo significa?* |
| **Unidade básica** | Subtópico com código (ex: `4.2`) | Entrada com definição formal |
| **Uso principal** | Classificar, indexar, tagear | Definir, padronizar, verificar |
| **Quem usa** | S07 (briefing), curadoria documental | S04 (auditoria), S03, S06, documentos formais |

**Exemplo prático — o termo "Interoperabilidade":**

- **Na taxonomia:** aparece como subtópico `4.2 — Interoperabilidade: FHIR, HL7,
  SNOMED, LOINC, terminologias`. Quando uma notícia sobre integração de sistemas
  de saúde entra no briefing, recebe a tag `🏷️ 4.2` — indicando *onde o assunto mora*.
- **No glossário:** aparece como entrada com definição normativa extraída da
  regulação brasileira — o que o termo *significa* formalmente no contexto
  institucional da DTD/SETIS/SES-DF.

A coexistência dos dois não é redundância. São usos diferentes do mesmo conceito.

**Regra para agentes de IA:**
- Classificar um item por tema → use esta taxonomia, atribua o código do
  subtópico mais específico disponível.
- Verificar ou citar a definição de um termo → use o `GLOSSARIO.md` do M01.
- Nunca substitua um pelo outro.

---

## Como usar esta taxonomia

### Para classificação de itens (briefing, documentos, projetos)

1. Identifique o assunto central do item
2. Localize a Parte mais adequada (I a VIII)
3. Desça ao capítulo (ex: `Cap. 3 — IA e ML em Saúde`)
4. Atribua o subtópico mais específico disponível (ex: `3.1`)
5. Se o item se encaixa em mais de um subtópico, liste todos separados por ` · `
6. Máximo de 3 tags por item para manter clareza

**Exemplo:**
> Notícia sobre startup que usa LLM para triagem de sintomas em UPA →
> `🏷️ 3.2 · 3.3 · 19.2`
> (IA clínica e triagem · LLMs na medicina · startups e healthtechs)

### Para navegação e curadoria

- Use os códigos de Parte para filtrar por grandes domínios
- Use os capítulos para agrupar conteúdo temático em relatórios
- Use os subtópicos para indexação fina em acervos documentais

---

## Estrutura

A taxonomia está organizada em 8 Partes e 24 capítulos:

| Parte | Tema | Capítulos |
|---|---|---|
| I | Fundamentos e Contexto | 1–2 |
| II | Tecnologias Habilitadoras | 3–6 |
| III | Modelos de Cuidado Digital | 7–10 |
| IV | Dados, Privacidade e Segurança | 11–12 |
| V | Medicina de Precisão e Ciências Ômicas | 13–14 |
| VI | Saúde Pública Digital e Equidade | 15–17 |
| VII | Regulação, Mercado e Inovação | 18–20 |
| VIII | Fronteiras Emergentes | 21–24 |

O arquivo principal é [`taxonomia.md`](./taxonomia.md).

---

## Navegação

| Arquivo | Conteúdo |
|---|---|
| [taxonomia.md](./taxonomia.md) | Estrutura completa da taxonomia |
| [INDICE.md](./INDICE.md) | Índice de arquivos do repositório |
| [backlog-versoes.md](./backlog-versoes.md) | Histórico de versões |

---

## Contexto institucional

**Unidade:** Diretoria de Transformação Digital — DTD
**Órgão:** Secretaria Executiva de Tecnologia da Informação em Saúde — SETIS
**Secretaria:** Secretaria de Estado de Saúde do Distrito Federal — SES-DF
