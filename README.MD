# 📊 TelecomX_BR – Análise de Evasão de Clientes

Este projeto realiza uma análise exploratória e preditiva dos dados de clientes da TelecomX, com o objetivo de identificar os principais fatores que levam à evasão (churn) e propor estratégias para retenção.

## 🎯 Objetivo

Investigar padrões de comportamento que indicam risco de cancelamento de serviços por parte dos clientes, utilizando técnicas de ciência de dados e visualização.

## 💾 Fonte de Dados

Os dados foram extraídos de uma API em formato JSON e tratados para análise. O conjunto inclui informações demográficas, serviços contratados, tipo de contrato, método de pagamento e valores cobrados.

## 🧪 Etapas da Análise

1. **Extração e Carregamento**
   - Importação via `requests` e transformação em DataFrame com `pandas`.

2. **Limpeza e Transformação**
   - Renomeação de colunas para português.
   - Tradução de valores categóricos (Sim/Não).
   - Verificação de valores nulos e inconsistências.

3. **Análise Exploratória (EDA)**
   - Visualização da distribuição de churn.
   - Relação entre evasão e variáveis como contrato, método de pagamento, tempo de permanência e serviços agregados.

4. **Modelagem Preditiva**
   - Aplicação de Random Forest para prever churn.
   - Interpretação dos resultados com SHAP.

## 📈 Principais Insights

- Clientes com **contratos mensais** e **serviço de fibra óptica** apresentam maior risco de evasão.
- O método de pagamento **cheque eletrônico** está fortemente associado ao churn.
- A maioria dos cancelamentos ocorre nos **primeiros 12 meses** de contrato.
- Clientes **idosos** e **sem dependentes** têm maior propensão ao cancelamento.
- **Cobranças mensais elevadas** também estão correlacionadas com maior evasão.

## 🛠️ Tecnologias Utilizadas

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellowgreen?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-blueviolet?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?logo=matplotlib&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-teal?logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-ff69b4?logo=scikit-learn&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-Statistical%20Models-lightgrey?logo=python&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-Model%20Interpretability-red?logo=python&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google%20Colab-Notebook-ffce44?logo=googlecolab&logoColor=black)

## 🚀 Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/TelecomX_BR.git
   ```
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Acesse o notebook via [Google Colab](https://colab.research.google.com/drive/1qMKtv_42G03BNsVHcillgB_iWtDlRdD3#scrollTo=KKQDrUHvIgzf&uniqifier=1)
4. Execute todas as células para visualizar os gráficos e resultados.

## 💡 Recomendações

- Criar campanhas de retenção para clientes com contratos mensais.
- Incentivar migração para contratos anuais ou bienais.
- Oferecer suporte personalizado nos primeiros meses de serviço.
- Investigar causas de insatisfação com o serviço de fibra óptica.

- Monitorar clientes com cobranças elevadas e oferecer benefícios.
