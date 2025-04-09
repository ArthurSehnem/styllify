# 🔍 Análise Preditiva do Gasto Anual de Clientes da Styllify
Este repositório contém uma análise exploratória e preditiva do comportamento de compra dos clientes da **Styllify**, com foco em entender **quais fatores realmente influenciam o gasto anual** — e como isso pode direcionar decisões estratégicas de negócio.

---

## 🛍️ Sobre a Styllify

A **Styllify** é uma marca que combina o melhor do físico com o digital: nossos clientes recebem consultoria de estilo personalizada nas lojas e, depois, continuam a jornada de compra pelo nosso **site** ou **aplicativo móvel**.

---

## ❓ Pergunta Estratégica

Durante o planejamento do próximo ciclo de orçamento, surgiu um debate entre os times de produto e marketing:

> **“Devemos continuar investindo igualmente no app e no site?”**

A dúvida é legítima — os dois canais demandam recursos. Mas, sem dados concretos, a discussão virou uma disputa de opiniões. Foi aí que os olhos se voltaram para os dados — e para mim.

---

## 🎯 Objetivo do Projeto

Este projeto busca responder, com base em dados reais de clientes:

- **Quem gasta mais na Styllify?**
- **Existe uma relação direta entre o uso do app ou do site e o gasto anual?**
- **Ou estamos ignorando fatores mais relevantes, como a fidelidade do cliente à marca?**

A missão é identificar **os verdadeiros motores de receita** do nosso modelo de negócio e orientar a empresa com base em evidências.

---

## 🧠 Metodologia

### 1. Dados Utilizados
A base de dados contém informações de comportamento de centenas de clientes, com as seguintes variáveis principais:

- `Avg. Session Length` – tempo médio por sessão
- `Time on App` – tempo total no aplicativo
- `Time on Website` – tempo total no site
- `Length of Membership` – **tempo de associação como cliente**
- `Yearly Amount Spent` – gasto anual (variável-alvo)

### 2. Análise Exploratória
Utilizei gráficos de dispersão, correlação e pairplots para investigar a relação entre variáveis e identificar possíveis padrões.

### 3. Modelagem
Apliquei uma **regressão linear multivariada** para prever o `Yearly Amount Spent` com base nas variáveis comportamentais.

### 4. Avaliação do Modelo
Foram utilizadas as métricas:
- **MSE** – Erro Quadrático Médio
- **MAE** – Erro Absoluto Médio
- **RMSE** – Raiz do Erro Quadrático Médio
- **R²** – Coeficiente de Determinação

---

## ✅ Resultados

A análise revelou um insight crucial:

> **Não é o tempo no app ou no site que mais influencia o gasto anual — e sim o tempo de associação com a Styllify.**

### Principais achados:
- **`Length of Membership`** apresentou a **correlação mais forte com o gasto anual**, sendo o fator mais relevante da análise.
- O **tempo no app** teve influência moderada, mas **não determinante**.
- O **tempo no site** teve **pouco ou nenhum impacto significativo**.
- O modelo obteve um **R² elevado**, mostrando que as variáveis selecionadas explicam bem o comportamento de gasto.

---

## 📌 Conclusão

Essa descoberta muda o foco da discussão estratégica:

- Investir em **fidelização e relacionamento de longo prazo com os clientes** tende a trazer mais retorno do que uma disputa direta entre plataformas digitais.
- O app e o site são canais importantes, mas atuam mais como **facilitadores de compra**, e não como os principais impulsionadores de receita.

**Recomendações:**
- Fortalecer o programa de fidelidade.
- Criar campanhas personalizadas para clientes antigos.
- Reavaliar os investimentos em mídia digital com base em dados reais de impacto.

---

## 🧰 Ferramentas Utilizadas

- `Python` – linguagem principal
- `pandas`, `numpy` – análise e manipulação de dados
- `matplotlib`, `seaborn` – visualizações
- `scikit-learn` – modelagem preditiva
