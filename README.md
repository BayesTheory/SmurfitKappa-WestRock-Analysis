# SmurfitWest: Análise de Séries Temporais (Python) e Visualização de Dados (R)

Este repositório contém duas análises distintas:
1.  Uma análise e previsão de séries temporais de dados de expedição (m²) usando Python (SARIMA e LSTM).
2.  Uma análise exploratória e visualização de dados de fluxo de caixa de fundos mútuos usando R (ggplot2).

*(Contexto opcional sobre Smurfit Kappa/WestRock, se relevante para os dados usados)*

## Conteúdo do Repositório

*   **`Expedicao_ML_TimeSeries_Py.ipynb`** (anteriormente `SMURFIT_KAPPA_ML.ipynb`):
    *   **Objetivo:** Realiza análise exploratória (tendência, sazonalidade) e prevê a série temporal "Expedição M2" (carregada de `ml.xlsx`).
    *   **Metodologia:** Compara um modelo estatístico tradicional (SARIMA) com um modelo de Deep Learning (Rede Neural LSTM) para forecasting [6]. Inclui decomposição da série, análise ACF/PACF e visualização dos resultados [2, 5].
    *   **Linguagem:** Python.

*   **`MutualFunds_DataViz_R.ipynb`** (anteriormente `SMURFIT_KAPPA_R.ipynb`):
    *   **Objetivo:** Explora e visualiza dados de fluxo de caixa líquido mensal para diferentes categorias de fundos mútuos (ações e títulos), carregados de `mutual_funds_cash_flow.xlsx`.
    *   **Metodologia:** Limpeza de dados, análise de correlação e criação de gráficos de barras empilhadas (usando `ggplot2`) mostrando o fluxo de caixa por tipo de título ao longo do tempo, facetado por ano.
    *   **Linguagem:** R.

## Tecnologias Utilizadas

*   **Python 3:**
    *   Bibliotecas: `pandas`, `matplotlib`, `statsmodels`, `seaborn`, `numpy`, `scikit-learn`, `tensorflow` (`keras`) [2, 6].
*   **R:**
    *   Bibliotecas: `dplyr`, `ggplot2`, `readxl`, `reshape2`, `scales`, `Hmisc`, `tidyr`, `zoo`.
*   **Ambiente:** Jupyter Notebook.

## Instalação e Execução

**Pré-requisitos:**
*   Python 3.x instalado (com pip).
*   R instalado.
*   Jupyter Notebook ou JupyterLab instalado.
*   Arquivos de dados: `ml.xlsx` e `mutual_funds_cash_flow.xlsx` (precisam estar no mesmo diretório ou o caminho no código ajustado).

**Instruções:**

1.  **Clone o Repositório:**
    ```
    git clone https://github.com/BayesTheory/SmurfitWest.git
    cd SmurfitWest
    ```
2.  **Ambiente Python:**
    *   Crie e ative um ambiente virtual (recomendado):
        ```
        python -m venv venv
        source venv/bin/activate # Linux/Mac
        # venv\Scripts\activate # Windows
        ```
    *   Instale as dependências Python. Crie um arquivo `requirements.txt` com o seguinte conteúdo:
        ```
        pandas
        matplotlib
        statsmodels
        seaborn
        numpy
        scikit-learn
        tensorflow
        openpyxl # Para ler arquivos .xlsx
        ```
    *   Instale usando pip:
        ```
        pip install -r requirements.txt
        ```
3.  **Ambiente R:**
    *   Abra o R ou RStudio.
    *   Instale as dependências R necessárias:
        ```
        # Se necessário, execute no console R:
        install.packages(c("dplyr", "ggplot2", "readxl", "reshape2", "scales", "Hmisc", "tidyr", "zoo"))
        ```
    *   Certifique-se de que o kernel do R esteja disponível no Jupyter (pode exigir `install.packages('IRkernel')` e `IRkernel::installspec()` no R).

4.  **Execute os Notebooks:**
    *   Inicie o Jupyter: `jupyter notebook` ou `jupyter lab`
    *   Abra os arquivos `.ipynb` e execute as células. Certifique-se de que os arquivos `.xlsx` estão acessíveis.


Link do Projeto: https://github.com/BayesTheory/SmurfitWest
