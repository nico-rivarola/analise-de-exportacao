# 📊 Projeto de Análise de Exportações  

Este projeto tem como objetivo realizar uma **análise completa de exportações** a partir de uma base fictícia de vendas, combinando **Python** (para exploração e pré-processamento dos dados) e **Power BI** (para a criação de dashboard interativo).  

---

## 🔹 1. Preparação dos Dados  
A base original foi fornecida em formato **Excel (.xlsx)**. As seguintes etapas foram realizadas:  

- **Padronização de colunas** → ajuste de nomes (remoção de acentos e espaços).  
- **Tratamento de datas** → conversão para formato `datetime`.  
- **Criação de métricas derivadas**:  
  - `Faturamento = Quantidade_Vendida × Preço_Unitário`  
  - `Pedido_Alto` → flag indicando pedidos acima da mediana.  
- **Limpeza de dados**: remoção de linhas inconsistentes e valores nulos em colunas críticas.  
- **Normalização** de variáveis numéricas para uso em análises preditivas (Scikit-learn).  

---

## 🔹 2. Análises com Python  
Foi desenvolvido um **mini-EDA (Exploratory Data Analysis)** para entender melhor os dados antes da modelagem e visualização.  

Principais pontos analisados:  
- Distribuição de faturamento por região.  
- Produtos com maior receita e volume.  
- Representantes de vendas com maior desempenho.  
- Identificação de sazonalidade nas vendas.  
- Preparação para modelos de **regressão (predição de faturamento)** e **classificação (pedidos altos vs. baixos)**.  

Bibliotecas utilizadas:  
```python, pandas, numpy, seaborn, matplotlib, scikit-learn```
## 🔹 3. Dashboard Interativo (Power BI)

Após o tratamento e exploração em Python, os dados foram carregados no Power BI para visualização.

📌 Principais elementos do dashboard:

- KPIs → Receita total (R$ 419,15 mi) e Volume total (193 mil unidades).

- Gráficos de tendência → Receita de exportações por período.

- Gráficos comparativos → Receita por produto e por região.

- Mapa geográfico → Distribuição global de exportações.

- Gráfico de pizza/donut → Percentual de participação por continente.

👉 O dashboard permite aplicar filtros de período e visualizar rapidamente os principais mercados e produtos da empresa.

## 🔹 4. Tecnologias Utilizadas

`Python → Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn`

`Power BI → Visualização e dashboard interativo`

`Excel → Base de dados`
## 🔹 5. Resultados Obtidos

- Identificação dos produtos com maior impacto na receita.

- Diversificação de mercados (Ásia, América do Norte e Europa representaram juntos 100% da receita).

- Evidência de sazonalidade em determinados períodos do ano.

- Preparação de base para análises preditivas de faturamento e classificação de pedidos.
