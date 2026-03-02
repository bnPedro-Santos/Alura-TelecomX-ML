# Telecom X - Parte 2 📊

## 🎯 Propósito
Este projeto tem como objetivo **prever o churn de clientes** de uma empresa de telecomunicações, utilizando técnicas de aprendizado de máquina. A análise busca identificar variáveis relevantes que influenciam a evasão e construir modelos capazes de antecipar quais clientes estão em risco de cancelar seus serviços.

---

## 🛠️ Preparação dos Dados
1. **Classificação das variáveis**  
   - **Numéricas**: idade, tempo de contrato, valor mensal, etc.  
   - **Categóricas**: tipo de serviço, forma de pagamento, presença de dependentes, etc.  

2. **Normalização e Codificação**  
   - Variáveis numéricas foram normalizadas para evitar escalas diferentes.  
   - Variáveis categóricas foram transformadas via *one-hot encoding*.  

3. **Separação dos dados**  
   - Conjunto de treino e teste (ex.: 70% treino, 30% teste).  
   - Uso de **SMOTE** para balancear a proporção de churners e não churners.  

4. **Justificativas de modelagem**  
   - **DummyClassifier** como baseline.  
   - **Logistic Regression** pela interpretabilidade e bom desempenho em recall.  
   - **KNN** para avaliar proximidade entre clientes.  
   - **Random Forest** e **XGBoost** pela capacidade de capturar relações complexas e variáveis importantes.  

---

## 📊 Análise Exploratória (EDA)
Durante a EDA foram gerados gráficos como:
- Distribuição de churn por tipo de contrato.  
- Relação entre valor mensal e probabilidade de churn.  
- Heatmap de correlação entre variáveis numéricas.  

**Insights principais:**
- Clientes com contratos mensais têm maior probabilidade de churn.  
- Valores mensais mais altos estão associados a maior evasão.  
- Variáveis como tempo de contrato e forma de pagamento são altamente relevantes.  
