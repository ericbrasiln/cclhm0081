---
name: cclhm0081-docencia
description: >
  Use esta skill para qualquer tarefa no repositório da disciplina CCLHM0081 —
  História da América Independente (UNILAB, Eric Brasil). Acione sempre que o
  trabalho envolver: criar ou editar arquivos .qmd (Quarto/RevealJS), produzir
  fichamentos ou sínteses bibliográficas, elaborar atividades pedagógicas, montar
  ou revisar cronogramas, commitar alterações no branch 2026_1, ou preencher
  templates da pasta templates-quarto/. Nunca inventar conteúdo histórico,
  bibliográfico ou atribuído a autores. Qualquer tarefa ligada à disciplina,
  ao repositório ou aos seus materiais deve acionar esta skill.
---

# SKILL — cclhm0081-docencia

## Contexto do projeto

Repositório de materiais da disciplina **CCLHM0081 — História da América
Independente**, ministrada por **Eric Brasil** no curso de Licenciatura em História
do Instituto de Humanidades e Letras da **UNILAB**.

**Site publicado:** `https://ericbrasil.com.br/cclhm0081/`

**URLs relevantes:**

| Recurso | URL |
|---|---|
| Página principal | `https://ericbrasil.com.br/cclhm0081/` |
| Ementa HTML | `https://ericbrasil.com.br/cclhm0081/ementa/ementa` |
| Ementa PDF | `https://ericbrasil.com.br/cclhm0081/ementa/ementa.pdf` |
| Calendário HTML | `https://ericbrasil.com.br/cclhm0081/ementa/calendario` |
| Calendário PDF | `https://ericbrasil.com.br/cclhm0081/ementa/calendario.pdf` |
| Slides aula N | `https://ericbrasil.com.br/cclhm0081/slides/aula-N/` |

**Estrutura do repositório:**

```
cclhm0081/                         ← raiz do repositório
├── .claude/
│   └── CLAUDE.md
├── bibliografia/
├── cclhm0081-docencia/            ← subpasta da skill
│   ├── leitura-bibliografia/
│   │   ├── questoes-apoio.md
│   │   └── resenha.md
│   ├── templates-quarto/
│   │   ├── template-html.qmd
│   │   ├── template-pdf.qmd
│   │   └── template-slides.qmd
│   └── SKILL.md
├── ementa/
│   ├── calendario_files/libs/
│   ├── ementa_files/libs/
│   ├── calendario.html
│   ├── calendario.md
│   ├── calendario.pdf
│   ├── ementa.html
│   ├── ementa.md
│   └── ementa.pdf
├── imgs/
├── index_files/
├── slides/
│   ├── aula-1/ … aula-16/        ← apresentações por aula
│   │   ├── index.qmd
│   │   ├── index.html
│   │   └── index_files/
│   ├── imgs/                      ← imagens e QR codes compartilhados
│   └── custom.scss
├── noticias/                      ← avisos e comunicados para a turma
│   └── AAAA-MM-DD_aulaX.md
├── atividades/
├── index.html
├── index.md
├── LICENSE.md
└── README.md
```

**Branch de trabalho ativo:** `2026_1`
**Branch consolidado:** `main` — nunca commitar diretamente.

---

## Bootstrap — início obrigatório de sessão

Ao iniciar qualquer tarefa neste repositório, executar **antes de qualquer alteração**:

```bash
git branch --show-current      # confirmar que está em 2026_1
git status                     # verificar estado atual
git log --oneline -5           # entender o histórico recente
```

Se não estiver no branch correto:

```bash
git checkout 2026_1
```

Ler sempre para contextualizar a sessão:

- `ementa/ementa.md` — objetivos, avaliação, conteúdo programático
- `ementa/calendario.md` — datas e temas de todas as aulas

---

## Calendário resumido — 2026.1

| Aula | Data | Módulo | Tema |
|:----:|------|:------:|------|
| 1 | 26/02/2026 | I | Quem escreve a história das Américas? |
| 2 | 05/03/2026 | I |  Atividade presencial - Cuba nos Malês! |
| 3 | 12/03/2026 | I | Revolução Americana e a República dos EUA |
| 4 | 19/03/2026 | I | Revolução de Santo Domingo e independência do Haiti |
| 5 | 26/03/2026 | I | A nação haitiana e seus impactos no mundo moderno |
| 6 | 02/04/2026 | I | Atividade remota |
| 7 | 09/04/2026 | I | Independências da América Hispânica |
| 8 | 16/04/2026 | I | Formação dos Estados Nacionais da América Latina |
| 9 | 23/04/2026 | II | Era das abolições I: Caribe |
| 10 | 30/04/2026 | II | Era das abolições III: Cuba, abolição e independência |
| 11 | 07/05/2026 | II | Avaliação presencial |
| 12 | 14/05/2026 | III | Revolução Mexicana de 1910 |
| 13 | 21/05/2026 | III | Populismo, autoritarismo e democracia no século XX |
| 14 | 28/05/2026 | III | Revolução Cubana de 1959 |
| — | 04/06/2026 | — | **Sem aula — Corpus Christi** |
| 15 | 11/06/2026 | III | Movimentos civis, direitos humanos e cidadania |
| 16 | 18/06/2026 | III | Aula de encerramento |

Horário: **quintas-feiras, 14h–17h**, Sala 11.

---

## Princípios inegociáveis

### 1. Nunca inventar conteúdo

Proibido produzir:

- informações históricas sem base textual
- argumentos ou interpretações atribuídos a autores sem o texto em mãos
- citações — mesmo paráfrases devem ter o texto como fonte
- referências bibliográficas não fornecidas pelo docente
- datas, dados ou exemplos por suposição

**Quando o texto não estiver disponível no contexto**, não simular leitura. Agir assim:

1. Informar: *"O texto [título] não foi fornecido. Para prosseguir, cole o conteúdo
   ou indique o caminho do arquivo no repositório."*
2. Oferecer o que pode ser feito com o material disponível.
3. Jamais preencher lacunas com inferências não declaradas.

### 2. Usar sempre a bibliografia indicada como base

- Partir da bibliografia da disciplina e dos textos fornecidos no repositório.
- Não inserir referências externas por iniciativa própria.
- Sugerir leituras adicionais **somente se solicitado explicitamente**.

### 3. Tom acadêmico de graduação em História

Escrever de forma: clara, formal, analítica, historicamente rigorosa.

Evitar: linguagem coloquial, simplificações indevidas, jargão desnecessário,
tom genérico, afirmações categóricas sem base, voz de assistente virtual.

---

## Produção de conteúdo

### Fichamentos e sínteses bibliográficas

Ao trabalhar com textos fornecidos, identificar quando possível:

- tema central e argumento principal
- conceitos-chave utilizados pelo autor
- recorte temporal e espacial
- fontes ou abordagem metodológica
- relevância para os debates da disciplina

O texto produzido deve ser útil para estudo, preparação de aula e debate em sala,
sem extrapolar o que o autor sustenta.

### Leitura de bibliografia

Para tarefas envolvendo leitura e análise de textos da disciplina, consultar os
arquivos de referência em `cclhm0081-docencia/leitura-bibliografia/`:

| Arquivo | Quando ler |
|---|---|
| `leitura-bibliografia/resenha.md` | Ao produzir resenha ou síntese de texto para uso do docente |
| `leitura-bibliografia/questoes-apoio.md` | Ao elaborar questões de leitura guiada para estudantes |

**Pré-requisito para ambos:** o texto deve estar disponível no contexto (PDF
fornecido ou conteúdo colado). Nunca simular leitura de texto ausente.
Sempre verificar a aula e o módulo correspondentes em `ementa/ementa.md`
antes de iniciar qualquer produção.

### Atividades pedagógicas

Estrutura mínima para toda atividade elaborada:

| Campo | Conteúdo |
|---|---|
| **Objetivo** | O que se espera que o estudante desenvolva |
| **Descrição** | O que será feito, em que formato |
| **Materiais** | Textos, fontes ou recursos necessários |
| **Orientações** | Como realizar a atividade |
| **Avaliação** | Critérios básicos de acompanhamento |

As atividades devem estar ancoradas na bibliografia da disciplina e estimular leitura,
reflexão, debate e análise histórica compatíveis com o nível de graduação.

---

## Diretrizes para arquivos Quarto (.qmd)

### Templates disponíveis

A pasta `templates-quarto/` contém os modelos base do projeto:

| Arquivo | Finalidade |
|---|---|
| `template-slides.qmd` | Apresentações RevealJS |
| `template-html.qmd` | Páginas e materiais HTML |
| `template-pdf.qmd` | Documentos para exportação PDF |

**Ao criar novos materiais:** sempre partir do template correspondente.

**Se os templates estiverem desatualizados:** ler os `index.qmd` existentes em
`slides/aula-N/` para confirmar o padrão de YAML e estrutura em uso.

### YAML frontmatter padrão — slides

```yaml
---
title: "Aula N: Título da aula"
date: "AAAA-MM-DD"
date-format: full
lang: pt-br
format:
  revealjs:
    theme: [default, ../custom.scss]
    slide-number: true
    incremental: false
    chalkboard:
      buttons: true
    footer: "Eric Brasil | <a href=https://ericbrasil.com.br/contact/>Entre em contato</a> | CCLHM0081 — História da América Independente"
    logo: https://raw.githubusercontent.com/ericbrasiln/cclhm0081/63cc875c152f361a14f723efbe6bd161f5aaf8b6/banner_logos_hist.png
author:
  - name: Eric Brasil
    orcid: 0000-0001-5067-8475
toc: false
---
```

Campos **ausentes** intencionalmente: `subtitle`, `email`, `affiliation`.

### Convenções de slides RevealJS

| Elemento | Sintaxe |
|---|---|
| Separador | `---` |
| Slide com título | `## Título {.center}` |
| Slide sem título | `## {.center}` |
| Background image + conteúdo | `## Título {background-image="url" background-opacity="0.X" .center}` |
| Background image full | `## {background-image="url"}` |
| Background iframe | `## {background-iframe="url" background-interactive="true"}` |
| Overlay em iframe | `::: {style="position: absolute; width: 40%; right: 0; ..."}` |
| Imagem simples | `![Legenda](url){width=X%}` |
| Imagem com link na legenda | `![[Texto do link](url-fonte)](url-imagem){width=X%}` |
| Citação | `>` blockquote + `(AUTOR, data, p. N)` na linha seguinte |
| Lista | `- item` (sem `*`) |

### Estrutura obrigatória de toda apresentação

1. **Primeiro slide:** QR code de acesso — `![Acesse a apresentação](../imgs/qrc_aulaN.png)`
2. **Conteúdo:** slides temáticos seguindo a ementa
3. **Último slide:** `## Bibliografia da aula {.center}` com lista das leituras obrigatórias

### Citações

Formato padrão em slides: `(AUTOR, data, p. N)`

Exemplo no blockquote:
```
> "Trecho da citação."

(SANTOS, 2014, p. 221)
```

Na bibliografia final, usar formato ABNT completo.

### QR codes

Gerar com `qrencode` para cada nova apresentação:

```bash
qrencode -o slides/imgs/qrc_aulaN.png -s 10 -m 2 "https://ericbrasil.com.br/cclhm0081/slides/aula-N/"
```

Commitar a imagem separadamente, antes dos slides:
```
[Claude Code] feat: adiciona QR code para slides da aula N
```

### Ao criar ou editar .qmd

- Reaproveitar o YAML, seções e padrões de organização já adotados no projeto
- Preservar o estilo do docente — evitar mudanças que descaracterizem o material
- Evitar excesso de texto por slide: favorecer exposição oral, leitura e debate
- Organizar conceitos e exemplos de forma progressiva e compreensível

---

## Fluxo de trabalho com Git

### Procedimento padrão

```
editar/criar arquivos
    → docente renderiza com quarto
    → Claude Code commita atomicamente
    → git push origin 2026_1
    → abrir PR de 2026_1 → main via gh pr create
```

### Commits

```bash
git status                  # verificar arquivos modificados
git diff                    # revisar o que mudou antes de commitar
git add <arquivos>          # nunca usar git add . sem revisar
git commit -m "[Claude Code] tipo: descrição breve

Co-Authored-By: Claude Sonnet 4.6 <noreply@anthropic.com>"
```

Nunca usar `git push --force`. Nunca commitar diretamente em `main`.

### Padrão de commits

| Tipo | Uso |
|---|---|
| `feat` | novo material ou arquivo criado |
| `fix` | correção de erro em arquivo existente |
| `docs` | atualização de documentação ou síntese |
| `refactor` | reorganização sem mudança de conteúdo |
| `chore` | ajustes técnicos, YAML, metadados |

### Commits atômicos

Cada commit deve conter uma mudança pequena, coerente e identificável. Exemplos:

```
[Claude Code] feat: adiciona QR code para slides da aula 4
[Claude Code] feat: adiciona slides da aula 4 — Revolução Haitiana
[Claude Code] refactor: atualiza template-slides.qmd
[Claude Code] fix: corrige link para ementa.pdf no index.md
```

Não misturar: criação de slides + atualização de template + edição de ementa no mesmo commit.

### Pull Requests

Todo push para `2026_1` deve ser seguido de PR para `main` via `gh pr create`.

O corpo do PR deve:
- Descrever as alterações por arquivo/seção
- Incluir tabela de commits quando houver mais de um
- Deixar explícito que foi criado pelo Claude Code
- Encerrar com `🤖 Criado com [Claude Code](https://claude.com/claude-code)`
- **Não incluir checklists** no corpo do PR

---

## Questões de apoio à leitura

Ao elaborar questões de apoio, ler `cclhm0081-docencia/leitura-bibliografia/questoes-apoio.md`
antes de iniciar. As regras abaixo são um resumo operacional.

### Número e formato

- Entre **5 e 8 questões** — o número depende da extensão e complexidade do texto
- Questões abertas e discursivas — nunca de múltipla escolha ou verdadeiro/falso
- Cada questão deve exigir síntese ou paráfrase — evitar respostas copiáveis ou sim/não
- A última questão pode articular o texto com o tema da aula

### YAML frontmatter

```yaml
---
title: "Questões de apoio à leitura: Autor (ano)"
author: "Eric Brasil"
date: today
date-format: full
lang: pt-BR
---
```

### Nomenclatura de arquivo

```
autor_ano_questoes-apoio.md        ← texto completo
autor_ano_questoes-PAGINAS.md      ← trecho específico (ex: autor_ano_questoes-25-54.md)
```

Salvar em `bibliografia/apoio/`.

### Corpo do documento

```markdown
**Autor, "Título abreviado", ano, pp. XX–XX**
Aula N | Tema da aula

---

1. Questão em parágrafo corrido.

2. Questão em parágrafo corrido.
```

Questões numeradas com `1.` simples — sem `**N.**`, sem blocos, sem seções temáticas.
Cada questão em parágrafo único, sem sub-itens.

### Material de apoio na ementa

Após gerar o PDF, incluir em `ementa/ementa.md` na aula correspondente:

```markdown
**Material de apoio**

* [Questões de apoio à leitura — Autor (ano)](../bibliografia/apoio/arquivo.pdf): roteiro com N perguntas sobre [...], para orientar a leitura e o debate em sala.
```

---

## Noticias — avisos para a turma

Comunicados sobre aulas ficam em `noticias/` com a nomenclatura `AAAA-MM-DD_aulaX.md`.

### YAML frontmatter obrigatório

```yaml
---
title: "Aviso: Aula N — DD/MM/AAAA"
subtitle: "CCLHM0081 - 2026.1"
author:
  - name: Eric Brasil
    email: profericbrasil@unilab.edu.br
    orcid: 0000-0001-5067-8475
    affiliation: Instituto de Humanidades e Letras - UNILAB
date: AAAA-MM-DD
description: "Informações sobre a Aula N de ..."
lang: pt-BR
date-format: long
format:
  html:
    toc: false
    logo: ../imgs/banner_logos_hist.png
  pdf:
    toc: false
    documentclass: article
    geometry:
      - top=3cm
      - bottom=3cm
      - left=3.5cm
      - right=3.5cm
    fontsize: 12pt
    colorlinks: true
---
```

### Rodapé obrigatório

Todo aviso deve terminar com:

```markdown
---

*Mensagem escrita com assistência do [Claude Code](https://claude.com/claude-code).*
```

---

## Regras de .gitignore

O `.gitignore` do repositório deve conter:

```gitignore
*_resenha.md

# PDFs dos textos da bibliografia (direitos autorais)
bibliografia/*.pdf
```

A regra `bibliografia/*.pdf` ignora os PDFs dos textos protegidos por direitos autorais,
mas **não afeta** `bibliografia/apoio/*.pdf` (materiais produzidos pelo docente),
que continuam rastreados normalmente.

---

## Convenções editoriais

- **Nomes de arquivo:** minúsculas com hífens — ex.: `aula-04-haiti.qmd`
- **Organização:** por aula ou unidade temática, não por tipo de arquivo
- **Antes de criar:** verificar se o conteúdo já existe no repositório
- **Antes de commitar:** revisar ortografia, gramática e coerência
- **Preservar:** comentários, metadados e estruturas YAML relevantes já existentes
- **Voz dos textos:** refletir o docente, não uma redação genérica de assistente

---

## Limites de atuação

Esta skill não deve:

- alterar a organização do repositório sem solicitação ou justificativa clara
- apagar conteúdo sem confirmação do docente
- substituir a voz docente por redação genérica
- inserir bibliografia, interpretações ou dados sem base nos materiais fornecidos
- simular leitura de textos não fornecidos no contexto

**Quando houver dúvida, a prioridade é:**

1. Preservar o que já existe
2. Trabalhar com o material efetivamente disponível
3. Explicitar limites em vez de improvisar conteúdo
