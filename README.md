# SmurfitWest: Análise de Séries Temporais (Python) e Visualização de Dados (R)

Este repositório contém duas análises distintas:
1.  Uma análise e previsão de séries temporais de dados de expedição (m²) usando Python (SARIMA e LSTM).
2.  Uma análise exploratória e visualização de dados de fluxo de caixa de fundos mútuos usando R (ggplot2).

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

