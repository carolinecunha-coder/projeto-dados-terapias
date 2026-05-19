# 📊 Data-Driven Wellness: Análise de Texto e PLN em E-books de Terapias Integrativas

[![Python](https://img.shields.io/badge/Python-3.11-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-3.0-dataframe.svg)](https://pandas.pydata.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Este projeto aplica conceitos de **Ciência de Dados** e **Processamento de Linguagem Natural (PLN)** para realizar a extração, tratamento e análise estatística do conteúdo textual de e-books autorais voltados para práticas integrativas (*Mindfulness* e *Reiki*). 

O objetivo principal é transformar dados não estruturados (arquivos PDF) em insights quantificáveis, validando de forma empírica e matemática se a distribuição dos termos reflete com precisão as propostas editoriais e conceituais de cada obra.

---

## 📑 Índice
* [Contexto do Projeto](#-contexto-do-projeto)
* [Arquitetura e Pipeline de Dados](#%EF%B8%8F-arquitetura-e-pipeline-de-dados)
* [Tecnologias e Ferramentas](#%EF%B8%8F-tecnologias-e-ferramentas)
* [Resultados e Insights de Negócio](#-resultados-e-insights-de-negocio)
* [Como Executar o Projeto](#-como-executar-o-projeto)

---

## 🎯 Contexto do Projeto

No mercado de bem-estar e saúde holística, a consistência teórica é fundamental para a autoridade do conteúdo. Este projeto nasceu da necessidade de auditar e visualizar o peso temático de dois e-books digitais. Através de algoritmos de contagem e filtros de ruído textual (*stop words*), conseguimos extrair a real "impressão digital" de cada livro.

---

## ⚙️ Arquitetura e Pipeline de Dados

O fluxo de processamento dos dados textuais seguiu as seguintes etapas:
1. **Ingestão:** Leitura dos arquivos binários PDF utilizando `PyPDF2`.
2. **Sanitização (Data Cleaning):** Aplicação de Expressões Regulares (`re`) para remover caracteres especiais, pontuações e padronizar o texto em *lowercase*.
3. **Processamento de PLN:** Filtragem customizada de tokens para eliminação de *stop words* (palavras gramaticais sem valor semântico como preposições e artigos).
4. **Análise Frequencial:** Estruturação dos dados com `Pandas` e contagem via `collections.Counter`.
5. **Visualização:** Geração de mapas de relevância visual com `WordCloud` e plotagem via `Matplotlib`.

---

## 🛠️ Tecnologias e Ferramentas

* **Python 3.11:** Linguagem base do projeto.
* **Jupyter Notebook (`.ipynb`):** Ambiente interativo para prototipagem e exibição dos outputs.
* **PyPDF2:** Extração robusta de texto de arquivos PDF.
* **Pandas:** Manipulação de dados e criação de DataFrames para análise tabular.
* **Matplotlib:** Renderização e salvamento dos outputs gráficos.
* **WordCloud:** Algoritmo de vetorização visual de palavras por frequência.

---

## 📈 Resultados e Insights de Negócio

### 🧠 1. E-book: Mindfulness & Foco
* **Métrica de Volume:** 16 páginas processadas.
* **Análise de Frequência:**
  * `atenção`: 16 ocorrências
  * `plena`: 15 ocorrências
  * `pensamentos`: 14 ocorrências
* **Insight Técnico:** A proximidade métrica entre *Atenção* e *Plena* valida estatisticamente que o conceito de "Atenção Plena" foi o fio condutor do livro, com foco secundário no gerenciamento de *Pensamentos*.

🖼️ **Visualização de Dados (Mindfulness):**
*(A imagem abaixo foi gerada pelo script e salva automaticamente na raiz do projeto)*
![Nuvem de Palavras - Mindfulness](nuvem_mindfulness.png)

### 🌅 2. E-book: Terapia Integrativa Reiki
* **Métrica de Volume:** 17 páginas processadas.
* **Análise de Frequência:**
  * `energia`: 23 ocorrências
  * `reiki`: 20 ocorrências
  * `chakra` / `chakras`: 25 ocorrências (combinadas)
* **Insight Técnico:** O predomínio isolado do termo *Energia* comprova que o foco técnico do e-book está centralizado na manipulação energética e no alinhamento dos centros de força (*Chakras*), mantendo a fidelidade ao método tradicional Usui.

🖼️ **Visualização de Dados (Reiki):**
*(A imagem abaixo foi gerada pelo script e salva automaticamente na raiz do projeto)*
![Nuvem de Palavras - Reiki](nuvem_reiki.png)

---

## 🚀 Como Executar o Projeto

*(Esta secção serve de guia técnico para que outras pessoas saibam como reproduzir o teu trabalho)*

### Pré-requisitos
Ter o Python 3.11+ instalado na máquina.

### 1. Clonar o repositório
```bash
git clone [https://github.com/carolinecunha-coder/projeto-dados-terapias.git](https://github.com/carolinecunha-coder/projeto-dados-terapias.git)
cd projeto-dados-terapias