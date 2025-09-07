 Análise Estratégica para o Sucesso Cinematográ

## Objetivo do Projeto

Este projeto realiza uma análise aprofundada de um dataset de filmes do IMDb para fornecer insights estratégicos e uma ferramenta preditiva para o estúdio PProductions. O objetivo é responder a perguntas de negócio chave para orientar a produção de futuros filmes de sucesso, utilizando técnicas de análise exploratória, engenharia de features, processamento de linguagem natural e machine learning.

---

## Estrutura do Repositório

- **/data/raw:** Contém o dataset original para análise (`desafio_indicium_imdb.csv`)
- **/data/processed:** Contém o dataset tratado utilizado na análise (`imdb_data_treated.csv`).
- **/models:** Contém o modelo de machine learning finalizado e salvo (`imdb_rating_predictor.pkl`).
- **/notebooks:** Contém o Jupyter Notebook `relatorio_analise_filmes.ipynb` com todo o fluxo de trabalho da análise.
- **README.md:** Este documento.
- **environment.yml:** Arquivo para recriação do ambiente Conda (método recomendado).
- **requirements.txt:** Lista de dependências para instalação via pip.

---

## Como Executar o Projeto

Siga os passos abaixo para replicar a análise em seu ambiente local.

**Pré-requisitos:**
- Git
- Conda (Miniconda ou Anaconda)

### Opção 1: Usando Conda (Método Recomendado)

Este método recria o ambiente de desenvolvimento exato utilizado no projeto, garantindo total reprodutibilidade.

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/felinjob/hollywood_analise.git
    cd hollywood_analise
    ```

2.  **Crie o ambiente Conda a partir do arquivo `environment.yml`:**
    ```bash
    conda env create -f environment.yml
    ```
    Este comando irá instalar automaticamente a versão correta do Python e todas as bibliotecas necessárias.

3.  **Ative o novo ambiente:**
    O nome do ambiente está definido dentro do arquivo `environment.yml`. Após a criação, ative-o com:
    ```bash
    conda activate nome_do_ambiente_no_yml
    ```

### Opção 2: Usando venv e pip

Se você não utiliza Conda, pode criar um ambiente usando as dependências listadas no `requirements.txt`.

1.  **Clone o repositório e navegue até a pasta:**
    ```bash
    git clone https://github.com/felinjob/hollywood_analise.git
    cd hollywood_analise
    ```

2.  **Crie e ative um ambiente virtual:**
    ```bash
    python3 -m venv venv
    source venv/bin/activate
    # No Windows, use: venv\Scripts\activate
    ```

3.  **Instale as dependências:**
    ```bash
    pip install -r requirements.txt
    ```

### Execução da Análise

Após ativar o ambiente (seja por Conda ou venv), inicie o Jupyter Notebook para visualizar e executar a análise:
```bash
jupyter notebook notebooks/relatorio_analise_filmes.ipynb