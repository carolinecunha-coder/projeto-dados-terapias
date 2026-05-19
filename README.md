# 📊 Data-Driven Wellness: Análise de Texto em E-books de Terapias Integrativas

Este projeto utiliza conceitos de **Ciência de Dados** e **Processamento de Linguagem Natural (PLN)** básico para extrair, limpar e analisar estatisticamente o conteúdo de e-books autorais focados em práticas integrativas (*Mindfulness* e *Reiki*). 

O objetivo principal é transformar dados textuais não estruturados (arquivos PDF) em insights quantificáveis, validando a consistência dos temas abordados através de tabelas de frequência e visualizações gráficas (Nuvens de Palavras).

## 🛠️ Tecnologias e Bibliotecas Utilizadas
* **Python 3.11** (Ambiente Virtual Isolado `.venv`)
* **Jupyter Notebooks** (`.ipynb`) para desenvolvimento interativo
* **PyPDF2**: Extração e leitura de texto em arquivos binários de PDF
* **Pandas**: Estruturação de dados em DataFrames e análise de frequência
* **Matplotlib**: Plotagem e renderização dos gráficos na tela
* **WordCloud**: Geração de mapas visuais de palavras-chave

## 📈 Resultados Encontrados

### 🧠 1. E-book: Mindfulness & Foco
* **Total de Páginas:** 16 páginas analisadas.
* **Métricas Principais:** Os termos dominantes foram *Atenção* (16x), *Plena* (15x) e *Pensamentos* (14x), comprovando estatisticamente o direcionamento prático do guia focado em regulação da atenção.

### 🌅 2. E-book: Terapia Integrativa Reiki
* **Total de Páginas:** 17 páginas analisadas.
* **Métricas Principais:** Os termos de maior relevância foram *Energia* (23x), *Reiki* (20x) e *Chakra* (15x), refletindo a forte fundamentação do material no equilíbrio do sistema energético.

## 🚀 Como Executar o Projeto
1. Certifique-se de ter o Python instalado.
2. Ative o ambiente virtual e instale as dependências:
   ```bash
   pip install PyPDF2 wordcloud matplotlib pandas ipykernel