# 📊 Previsão de Churn — Telecom X

## 📌 Visão Geral

Este projeto tem como objetivo prever a evasão de clientes (**churn**) de uma empresa de telecomunicações, utilizando técnicas de **Machine Learning**. A solução foi desenvolvida com foco em:

- Análise exploratória
- Preparação de dados
- Escolha e avaliação de modelos
- Geração de insights para retenção de clientes

---

## 🎯 Objetivo

Você foi contratado como assistente de análise de dados na **Telecom X** e fará parte do projeto **"Churn de Clientes"**.  
A empresa enfrenta um alto índice de cancelamentos e precisa entender os fatores que levam à perda de clientes.

Seu desafio será:

- Coletar, tratar e analisar os dados
- Utilizar Python e suas principais bibliotecas
- Auxiliar a equipe de Data Science na criação de modelos preditivos
- Gerar estratégias para reduzir a evasão de clientes

### 🧪 O que você vai praticar:

- ✅ Importar e manipular dados de uma API de forma eficiente  
- ✅ Aplicar conceitos de ETL (Extração, Transformação e Carga)  
- ✅ Criar visualizações estratégicas para identificar padrões e tendências  
- ✅ Realizar uma Análise Exploratória de Dados (EDA) e gerar insights  

---

## 🧩 Etapas do Projeto

1. Importação e limpeza de dados  
2. Análise exploratória (EDA)  
3. Tratamento de variáveis categóricas  
4. Normalização de dados  
5. Construção e avaliação de modelos  
6. Exportação do modelo final  

---

## 🤖 Modelos Avaliados

### 1. **Regressão Logística**
- **Accuracy:** 79,35%  
- **Precision:** 63,52%  
- **Recall:** 52,14%  
- **F1 Score:** 57,27%  
- **ROC AUC:** 0,8432  

### 2. **Random Forest**
- **Accuracy:** 78,14%  
- **Precision:** 61,87%  
- **Recall:** 45,99%  
- **F1 Score:** 52,76%  
- **ROC AUC:** 0,8129  

> 🔎 **Conclusão:** A **Regressão Logística** apresentou melhor performance geral, com destaque para o **Recall** e a **área sob a curva ROC**, sendo escolhida como modelo final.

---

## 📌 Principais Variáveis Relevantes

- Tipo de contrato (mensal → maior churn)
- Método de pagamento (boleto e débito automático → maior churn)
- Adesão a serviços adicionais (ausência de suporte técnico ou segurança → maior churn)
- Tipo de serviço de internet
- Valor mensal da fatura

---

## 💡 Estratégias de Retenção Sugeridas

- Incentivar contratos de maior duração (trimestral/anual)  
- Oferecer pacotes com serviços de segurança e suporte  
- Monitorar mensalmente os clientes com maior risco e agir com campanhas direcionadas  

---

## 💾 Exportação do Modelo

O modelo final foi salvo utilizando a biblioteca `joblib`:

```python
import joblib
joblib.dump(modelo_lr, 'modelo_regressao_logistica.pkl')
