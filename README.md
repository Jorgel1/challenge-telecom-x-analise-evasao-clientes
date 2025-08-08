# 📊 Previsão de Churn — Telecom X

## 📌 Visão Geral
Este projeto tem como objetivo prever a evasão de clientes (churn) de uma empresa de telecomunicações, utilizando técnicas de *machine learning*. A solução foi desenvolvida com foco na análise exploratória, preparação de dados, escolha de modelo e avaliação preditiva.

---

## 🎯 Objetivo
**Telecom X – Parte 2: Prevendo Churn**

## 🎯 Missão
Sua nova missão é desenvolver modelos preditivos capazes de prever quais clientes têm maior chance de cancelar seus serviços.

A empresa quer antecipar o problema da evasão, e cabe a você construir um pipeline robusto para essa etapa inicial de modelagem.

---

## 🧠 Objetivos do Desafio

- Preparar os dados para a modelagem (tratamento, *encoding*, normalização)
- Realizar análise de correlação e seleção de variáveis
- Treinar dois ou mais modelos de classificação
- Avaliar o desempenho dos modelos com métricas
- Interpretar os resultados, incluindo a importância das variáveis
- Criar uma conclusão estratégica apontando os principais fatores que influenciam a evasão

---

## 🧰 O que você vai praticar

✅ Pré-processamento de dados para Machine Learning  
✅ Construção e avaliação de modelos preditivos  
✅ Interpretação dos resultados e entrega de insights  
✅ Comunicação técnica com foco estratégico

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

### 1. Regressão Logística
- **Accuracy:** 79,35%  
- **Precision:** 63,52%  
- **Recall:** 52,14%  
- **F1 Score:** 57,27%  
- **ROC AUC:** 0,8432

### 2. Random Forest
- **Accuracy:** 78,14%  
- **Precision:** 61,87%  
- **Recall:** 45,99%  
- **F1 Score:** 52,76%  
- **ROC AUC:** 0,8129

### 🔎 Conclusão:
A **Regressão Logística** apresentou melhor performance geral, com destaque para o *Recall* e a área sob a curva ROC, sendo escolhida como modelo final.

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
