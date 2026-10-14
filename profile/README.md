# bncc.dev

**A Base Nacional Comum Curricular como infraestrutura aberta.**

A BNCC é obrigatória em toda escola brasileira. Ela circula como PDF de 600 páginas e planilhas do MEC. Aqui ela é dado estruturado, verificado caractere a caractere contra os documentos oficiais e rastreável registro a registro. Serve a quem constrói ferramentas educacionais, pesquisa currículo ou precisa citar a norma com precisão.

## Projetos

| Repositório | O que é |
|---|---|
| **[bncc-dados](https://github.com/bncc-dev/bncc-dados)** | O dataset canônico: 1.721 aprendizagens em JSON, SQLite e CSV. Cada registro traz a fonte oficial e a página. O pipeline de extração é reprodutível e roda no CI a cada mudança. [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.21625233.svg)](https://doi.org/10.5281/zenodo.21625233) |
| **[bncc-pacotes](https://github.com/bncc-dev/bncc-pacotes)** | O dataset consumível em uma linha: pacotes npm e PyPI, mais um servidor MCP que dá ao seu agente de IA acesso ao currículo. |
| **[bncc-benchmark](https://github.com/bncc-dev/bncc-benchmark)** | Benchmark aberto de alucinação de LLMs sobre a BNCC: 15.300 respostas de 17 modelos, com metodologia e dados brutos públicos. O conjunto held-out fica privado para evitar contaminação. |

Consulta e navegação em **[bncc.dev](https://bncc.dev)**.

## Uso rápido

```bash
npm install @bncc/dados     # JavaScript e TypeScript
pip install bncc            # Python
npx -y @bncc/mcp            # servidor MCP para agentes de IA
```

```bash
claude mcp add bncc -- npx -y @bncc/mcp
```

## O compromisso

**O que é aberto é irrevogavelmente aberto.** Dados sob CC BY 4.0, código sob MIT, sem cadastro e sem chave de API. Nada sai da coluna aberta para a comercial. O caminho inverso é sempre permitido.

O pipeline de extração é público. O CI reproduz o dataset inteiro a partir das fontes oficiais a cada mudança e reprova qualquer divergência.

## Contribuir

Correções de dado exigem fonte oficial: documento do MEC ou CNE, com página. O CI aplica a regra automaticamente. Comece pelas [good first issues](https://github.com/bncc-dev/bncc-dados/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) ou abra uma [discussão](https://github.com/bncc-dev/bncc-dados/discussions).

Mantido pela [Profy Tecnologias Educacionais Ltda](https://profy.com.br) (CNPJ 53.669.787/0001-45, Brasília). Contato: contato@bncc.dev · [Sobre o projeto](https://bncc.dev/sobre/)

---

## In English

**Brazil's National Common Curricular Base (BNCC) as open infrastructure.** The BNCC defines what every student in Brazilian basic education has the right to learn, and it is mandatory for every school in the country. The Ministry of Education publishes it as a 600-page PDF and spreadsheets. Here it is structured data, verified character by character against the official documents and traceable record by record.

| Repository | What it is |
|---|---|
| **[bncc-dados](https://github.com/bncc-dev/bncc-dados/blob/main/README.en.md)** | The canonical dataset: 1,721 learning objectives in JSON, SQLite and CSV, each with its official source and page. Reproducible extraction pipeline, run in CI on every change. |
| **[bncc-pacotes](https://github.com/bncc-dev/bncc-pacotes/blob/main/README.en.md)** | The dataset in one line: npm and PyPI packages, plus an MCP server that gives AI agents access to the curriculum. |
| **[bncc-benchmark](https://github.com/bncc-dev/bncc-benchmark)** | Open benchmark of LLM hallucination about the BNCC, with methodology and raw data (in Portuguese). The held-out set stays private to avoid contamination. |

Data under CC BY 4.0, code under MIT, no sign-up and no API key. What is open stays open. Maintained by [Profy Tecnologias Educacionais Ltda](https://profy.com.br) (CNPJ 53.669.787/0001-45, Brasília, Brazil). Contact: contato@bncc.dev · [About the project](https://bncc.dev/en/about/)
