# Workshop: Data Science Aplicada ao Futebol (Modelo de xG)

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/PureVice/workshop-data-science-for-soccer/blob/main/baseline_xg_fame25.ipynb)

Este repositório contém os materiais e códigos desenvolvidos durante o workshop de **Data Science Aplicada ao Futebol**. O foco principal deste projeto é a construção, do zero, de um modelo de **Expectativa de Gols (xG)** utilizando Python e dados reais de partidas de futebol.

## ⚽ Sobre o Projeto

O objetivo deste notebook é desmistificar as métricas avançadas de futebol, ensinando passo a passo como processar dados de rastreamento (tracking data) e eventos para criar um modelo estatístico capaz de prever a probabilidade de um chute resultar em gol.

### Tópicos Abordados:
- **Coleta e Carregamento de Dados:** Importação de datasets de chutes (Shots) da Copa do Mundo de 2022.
- **Engenharia de Atributos (Feature Engineering):**
  - Cálculo da **Distância** euclidiana até o gol.
  - Cálculo do **Ângulo** de visão para o gol (baseado em trigonometria).
- **Visualização de Dados:**
  - Plotagem de mapas de chutes e gols usando a biblioteca `mplsoccer` e o script auxiliar `gandula_view`.
  - Análise de densidade de finalizações.
- **Modelagem Estatística:**
  - Implementação de uma **Regressão Logística** com `scikit-learn`.
  - Ajuste de coeficientes para calcular a probabilidade de gol.
- **Avaliação de Modelo:**
  - Uso da métrica **ROC AUC** para validar a eficácia do modelo.

## 🛠️ Tecnologias e Bibliotecas

O projeto foi desenvolvido em **Python 3** utilizando as seguintes bibliotecas:

* **Manipulação de Dados:** `pandas`, `numpy`
* **Visualização:** `matplotlib`, `seaborn`, `mplsoccer`
* **Machine Learning:** `scikit-learn`
* **Utilitários:** `gdown` (para download dos datasets)

## 📂 Estrutura do Repositório

```bash
workshop-data-science-for-soccer/
│
├── baseline_xg_fame25.ipynb   # Notebook principal com o código e explicações
├── gandula_view.py            # Script auxiliar para visualização de campo (baixado via gdown no notebook)
└── README.md                  # Documentação do projeto
