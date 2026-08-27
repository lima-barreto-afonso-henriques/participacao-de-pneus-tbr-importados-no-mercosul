<!--
  COMO USAR ESTE TEMPLATE
  1. Copie este arquivo para README.md na raiz do novo projeto.
  2. Substitua os trechos entre [colchetes] pelo conteúdo real do projeto.
  3. Seções marcadas "(opcional)" podem ser removidas se não fizerem
     sentido para o projeto (ex.: "Artigo de referência" só se aplica a
     projetos que replicam uma metodologia publicada).
  4. Apague este bloco de comentário antes de publicar.
-->

# [Nome do Projeto]

[Uma frase descrevendo o que o projeto faz e para quem — "o que é isso?"]

---

## 📖 Referência / Contexto (opcional)

Se o projeto replica ou se baseia numa metodologia publicada, cite-a
aqui:

> [Autor(es). (Ano). *Título*. Periódico/Fonte. DOI ou link.]

A regra deste tipo de projeto costuma ser: **a linha de base segue a
referência à risca**; qualquer etapa em que o projeto vai além dela (ver
[Extensões](#-extensões--decisões-de-projeto-opcional)) fica marcada
explicitamente, para que a comparação entre "replicação" e "proposta
própria" seja sempre clara.

Se o projeto não tiver uma referência externa, troque esta seção por um
parágrafo de contexto: por que o projeto existe, que problema resolve.

---

## 🗂️ Estrutura do repositório

```
├── scripts/
│   ├── 00_functions/         # código compartilhado por todos os scripts
│   │   ├── 00_setup.R        # pacotes e opções globais
│   │   ├── 01_utils.R        # funções utilitárias
│   │   └── 02_themes.R       # paleta de cores e temas ggplot2
│     
│   ├── 01_data_prep/         # ingestão e limpeza
│   ├── 02_eda/               # análise exploratória
│   ├── 03_analysis/          # modelagem / análise principal
|   ├── 03_models/
│   └── 05_outputs/           # exportação de figuras e tabelas finais
│
├── data/
│   ├── raw/                  # dados brutos (não versionados)
│   ├── processed/            # dados intermediários (.rds)
│   └── outputs/              # artefatos finais (.rds, figuras, tabelas)
│
├── docs/                     # documentação didática (dicionário de dados etc.)
└── README.md
```

> Ajuste os nomes de subpasta conforme as etapas reais do projeto —
> o que não muda é `00_functions/` e a leitura em ordem numérica.

---

## 🧭 Metodologia / Etapas do projeto

| Etapa | O que é feito | Script |
|---|---|---|
| [Nome da etapa 1] | [breve descrição] | `NN_nome_do_script.R` |
| [Nome da etapa 2] | [breve descrição] | `NN_nome_do_script.R` |
| [Nome da etapa 3] | [breve descrição] | `NN_nome_do_script.R` |

Se o projeto segue uma referência publicada, uma coluna extra "Seção do
artigo" ajuda a rastrear cada decisão até o texto original.

---

## 🧪 Extensões / Decisões de projeto (opcional)

Se o projeto tem escolhas metodológicas próprias — que vão além de uma
referência externa, ou que não são óbvias a partir do código — documente
aqui o quê e o porquê:

- **[Nome da extensão 1]** — [o que muda em relação à abordagem padrão, e
  por que essa escolha foi feita].
- **[Nome da extensão 2]** — [idem].

---

## ▶️ Como reproduzir

**Requisitos:** [versão do R / linguagem], e os pacotes usados pelo
projeto (ex.: instalados via `pacman::p_load()` ou `renv::restore()`).

1. Clone o repositório e abra-o como projeto (`.Rproj`, para que
   `here::here()` resolva os caminhos corretamente).
2. [Onde colocar os dados de entrada, se o repositório não incluir dados
   brutos.]
3. Rode os scripts em ordem numérica dentro de cada pasta. Todos começam
   com `source(here::here("scripts", "00_functions", "00_setup.R"))`.
4. Os artefatos (tabelas, modelos, figuras) são salvos em
   `data/outputs/`.

---

## 📊 Resultados principais (opcional)

[Uma tabela ou 2-3 frases com o resultado central do projeto — números
que alguém abrindo o repositório pela primeira vez precisa saber antes de
mergulhar no código.]

---

## ✍️ Autor

**[Seu nome]** — [afiliação/instituição]

## 📄 Como citar este repositório (opcional)

```bibtex
@misc{[chave_da_citacao],
  title  = {[Nome do Projeto]},
  author = {[Seu nome]},
  year   = {[Ano]},
  url    = {[URL do repositório]}
}
```

## 📜 Licença

[Defina a licença do repositório (ex.: MIT, CC-BY-4.0) antes de publicar.]
