---
description: Renderiza todos os documentos da disciplina com quarto render
allowed-tools: Bash(quarto render:*)
---

Renderize todos os documentos da disciplina CCLHM0081 com `quarto render` seguindo as regras abaixo.

## Arquivos a renderizar e formatos

| Arquivo | Formatos |
|---|---|
| `ementa/ementa.md` | HTML + PDF (frontmatter já define ambos) |
| `ementa/calendario.md` | HTML + PDF (frontmatter já define ambos) |
| `index.md` | HTML apenas (frontmatter define `format: html`) |
| `noticias/*.md` | HTML + PDF (frontmatter já define ambos) |
| `bibliografia/apoio/*_questoes-apoio.md` | **PDF apenas** (`--to pdf`) |

## Instruções

1. Execute cada render na ordem da tabela acima.
2. Para `noticias/*.md` e `bibliografia/apoio/*_questoes-apoio.md`, itere sobre todos os arquivos correspondentes ao padrão glob — pode haver zero ou vários.
3. Para as questões de apoio use obrigatoriamente o flag `--to pdf`.
4. Reporte o resultado de cada render (sucesso ou erro) ao final.
5. Não faça commit, não faça push — apenas renderize.

## Estado atual dos arquivos

Notícias disponíveis: !`ls noticias/*.md 2>/dev/null || echo "(nenhuma)"`

Questões de apoio disponíveis: !`ls bibliografia/apoio/*_questoes-apoio.md 2>/dev/null || echo "(nenhuma)"`
