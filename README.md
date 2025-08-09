# Análise de Salários na Área de Dados

Este repositório contém uma análise exploratória de dados sobre salários em diversas profissões da área de dados, como Cientista de Dados, Engenheiro de Dados e Analista de Dados. O projeto foi desenvolvido como parte dos estudos da Imersão de Dados da Alura.

O notebook `DS_Alura.ipynb` detalha todo o processo, desde a importação e limpeza dos dados até a criação de visualizações interativas para extrair insights.

## 📂 Dataset

O conjunto de dados utilizado foi obtido publicamente e contém informações sobre salários de profissionais de dados, incluindo:

* Ano de trabalho (`ano`)
* Nível de senioridade (`senioridade`)
* Tipo de contrato (`contrato`)
* Cargo (`cargo`)
* Salário em USD (`usd`)
* Localização da empresa e residência do funcionário (`localizacao`, `residencia`)
* Modalidade de trabalho (remoto, presencial, híbrido)
* Tamanho da empresa (`tamanho`)

O dataset é carregado diretamente da seguinte URL no notebook:
```bash
https://raw.githubusercontent.com/guilhermeonrails/data-jobs/refs/heads/main/salaries.csv
```

## 🚀 Tecnologias Utilizadas

Este projeto foi desenvolvido inteiramente em Python, utilizando as seguintes bibliotecas principais:

-   **Pandas:** Para manipulação, limpeza e análise dos dados.
-   **NumPy:** Para operações numéricas.
-   **Matplotlib & Seaborn:** Para a criação de gráficos estáticos e estilizados.
-   **Plotly Express:** Para a criação de visualizações de dados interativas.
-   **PyCountry:** Para a conversão de códigos de países (ISO 3166-1 alpha-2 para alpha-3) para a plotagem do mapa.
-   **Streamlit:** O notebook também inclui o código base para a construção de um dashboard interativo.

## 🛠️ Etapas do Projeto

A análise foi dividida em várias etapas dentro do Jupyter Notebook:

1.  **Carregamento e Exploração Inicial:**
    -   Importação do dataset a partir de uma URL.
    -   Uso de funções como `.head()`, `.info()`, `.describe()` e `.shape` para uma primeira avaliação da estrutura e conteúdo dos dados.

2.  **Limpeza e Preparação dos Dados:**
    -   Renomeação das colunas para o português para facilitar a compreensão.
    -   Tradução e padronização de valores categóricos (ex: `SE` para `Sênior`, `FT` para `Tempo Integral`).
    -   Verificação e tratamento de valores ausentes (`NaN`).
    -   Correção do tipo de dado da coluna `ano` de `float` para `int`.

3.  **Visualização de Dados e Análise:**
    -   Criação de gráficos de barras para analisar a média salarial por nível de senioridade.
    -   Desenvolvimento de histogramas e boxplots para entender a distribuição dos salários.
    -   Criação de gráficos de pizza para visualizar a proporção entre as modalidades de trabalho (Presencial, Remoto e Híbrido).
    -   Geração de um mapa coroplético para comparar a média salarial de Cientistas de Dados entre diferentes países.

## 📊 Dashboard Interativo com Streamlit

A última parte do projeto consiste no desenvolvimento de um dashboard interativo com a biblioteca **Streamlit**. O código para a aplicação (`app.py`) permite que o usuário filtre os dados por:
-   Ano
-   Senioridade
-   Tipo de Contrato
-   Tamanho da Empresa

O dashboard exibe métricas-chave (KPIs) e os principais gráficos gerados na análise de forma dinâmica.

## 🏁 Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/leomatiazzz/ImersaoDS.git
    ```
2.  **Navegue até a pasta do projeto:**
    ```bash
    cd ImersaoDS
    ```
3.  **Instale as dependências:**
    *(Recomendado criar um ambiente virtual primeiro)*
    ```bash
    pip install -r requirements.txt
    ```
4.  **Abra o Jupyter Notebook:**
    ```bash
    jupyter notebook DS_Alura.ipynb
    ```
