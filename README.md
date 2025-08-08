# 📊 Projeto Churn de Clientes – Telecom X

Bem-vindo ao projeto de análise de evasão de clientes (Churn) da empresa **Telecom X**. Este repositório contém a análise exploratória realizada sobre os dados de clientes da empresa com o objetivo de entender os principais fatores que contribuem para o cancelamento dos serviços.

---

## 📌 Objetivo

A **Telecom X** tem enfrentado um alto índice de cancelamento de clientes. Este projeto tem como objetivo analisar os dados fornecidos pela empresa, tratar as inconsistências e aplicar técnicas de **Análise Exploratória de Dados (EDA)** para extrair insights valiosos sobre o comportamento dos clientes que evadem. 

---

## 🛠️ Tecnologias Utilizadas

- Python 3.10+
- Pandas
- NumPy
- Matplotlib & Seaborn
- Jupyter Notebook

---

## 📂 Estrutura do Repositório

```bash
├── Challenge_ETL_telecomX.ipynb              # Notebook com o pipeline de ETL e análise exploratória
├── dataset/telecomx_data_gold.csv            # Pasta com os dados tratados 
├── requirements.txt                          # Bibliotecas necessárias para rodar o projeto
└── README.md                                 # Este arquivo
```

---

## 🔍 Etapas Realizadas

### 1. **Importação e Tratamento dos Dados**
- Extração de dados de uma API em formato JSON.
- Normalização das colunas e correção de tipos de dados.
- Preenchimento e tratamento de valores nulos.
- Criação de novas features, como `Daily_Charges`.

### 2. **Análise Exploratória de Dados (EDA)**
- Análise da variável alvo `Churn`, que representa se o cliente evadiu ou não.
- Geração de gráficos para entender o comportamento dos clientes por:
  - Tipo de contrato
  - Tempo de permanência (`tenure`)
  - Serviços contratados
  - Tipo de pagamento
  - Fatura diária

### 3. **Análise de Correlação**
- Verificação da relação entre variáveis e a variável alvo.
- Criação de mapa de calor e gráficos de dispersão.

---

## 📈 Principais Insights

- Clientes com contratos mensais têm maior chance de evadir.
- Menor tempo de permanência está fortemente relacionado ao churn.
- A ausência de serviços como suporte técnico, backup e segurança online está associada ao cancelamento.
- Clientes com faturas diárias mais altas também demonstram maior churn.
- Cobrança eletrônica (Paperless Billing) também está relacionada a maior evasão.

---

## ✅ Conclusões e Recomendações

- **Incentivar contratos de longo prazo** com benefícios adicionais.
- **Oferecer pacotes combinados** de serviços essenciais com desconto.
- **Foco em retenção nos primeiros meses de uso**, pois o churn ocorre majoritariamente no início do ciclo.
- **Criar campanhas de reengajamento** para perfis com alto risco de churn.

---

## 💡 Próximos Passos

- Aplicar **modelos preditivos** após balanceamento da variável `Churn`.
- Explorar técnicas como **SMOTE** e validação cruzada.
- Construir dashboards interativos para acompanhamento contínuo de churn.

---

