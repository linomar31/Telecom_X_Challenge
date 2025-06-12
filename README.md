# Telecom_X_Challenge
Projeto "Churn de Clientes". Análise de evasão de clientes da Empresa Telecom X.
# 📊 Análise de Evasão de Clientes (Churn)

Este projeto tem como objetivo analisar os padrões de evasão de clientes (churn) de uma empresa de serviços de telecomunicações, utilizando dados reais de clientes e técnicas de análise exploratória e modelagem preditiva.

## 📁 Estrutura do Projeto

- `notebook.ipynb`: Notebook com todo o processo de limpeza, análise e modelagem.
- `Relatorio_Churn_Analysis.md`: Relatório técnico em Markdown com todas as etapas descritas.
- `data/`: Pasta para armazenar os dados utilizados (não incluída por padrão).
- `README.md`: Documentação do projeto.

---

## 🚀 Objetivo

Entender os principais fatores associados ao cancelamento de serviços por parte dos clientes, ajudando a empresa a tomar decisões estratégicas para reduzir a evasão.

---

## 🧼 Etapas Realizadas

### 1. Limpeza e Preparação de Dados

- Extração de colunas aninhadas (JSON aninhado).
- Criação de colunas como `MonthlyCharges`, `TotalCharges`, `Contas_Diarias`.
- Conversão de colunas para tipos numéricos adequados.
- Preenchimento de valores ausentes e tratamento de inconsistências.

### 2. Análise Exploratória

- Estatísticas descritivas (média, mediana, desvio padrão).
- Visualizações de churn por variáveis categóricas (gênero, tipo de contrato, método de pagamento).
- Boxplots para variáveis numéricas (`tenure`, `TotalCharges`) com separação por churn.

### 3. Modelagem Preditiva

- Codificação de variáveis categóricas.
- Separação de dados em treino e teste.
- Criação e avaliação de um modelo `RandomForestClassifier` para prever a evasão.

---

## 📌 Principais Insights

- Clientes com contratos mensais têm maior taxa de evasão.
- Baixo tempo de permanência (`tenure`) e menor faturamento (`TotalCharges`) estão fortemente associados ao churn.
- Certos métodos de pagamento, como boleto, estão relacionados a maior risco de evasão.

---

## ✅ Recomendações

- Criar campanhas para incentivar contratos mais longos.
- Identificar e abordar clientes com baixo tempo de casa.
- Monitorar métodos de pagamento e oferecer alternativas mais estáveis.

---

## 📚 Requisitos

- Python 3.10+
- Bibliotecas: `pandas`, `seaborn`, `matplotlib`, `sklearn`
