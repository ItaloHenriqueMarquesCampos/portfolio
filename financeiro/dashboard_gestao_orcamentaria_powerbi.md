# 💼 **DASHBOARD DE GESTÃO ORÇAMENTÁRIA**

---

![g_orcamento](https://github.com/user-attachments/assets/80c0a302-90b8-4e9a-a755-8b4395eb4389)

---

## 🚀 **VISÃO GERAL**

Neste projeto foi desenvolvido um *Dashboard de Gestão Orçamentária no Power BI*, com base em dados extraídos de planilhas em *Excel*, tratados no *Power Query*.

O objetivo é automatizar o acompanhamento do orçamento da empresa, permitindo comparar valores planejados e realizados, identificar desvios e apoiar decisões financeiras de forma ágil.

---

## 📂 **FONTE DE DADOS**

- 📄 **Base única:** *Excel*

### 📊 Estrutura dos dados:

- **Tabela de Orçamento:**  
  - Mês  
  - Centro de custo  
  - Valor orçado  

- **Tabela de Realizado:**  
  - Mês  
  - Centro de custo  
  - Valor realizado  

---

## 🎯 **OBJETIVO DO DASHBOARD**

Analisar a performance orçamentária com foco em:

- 💰 *Valor Orçado*  
- 💸 *Valor Realizado*  
- 📊 *Saldo (Orçado - Realizado)*  
- 🎯 *Aderência ao orçamento*  

---

## ❓ **PERGUNTAS DE NEGÓCIO**

1. **Qual o total orçado vs realizado no período?**  
2. **Qual o saldo disponível ou excedido?**  
3. **Quais departamentos mais estouram o orçamento?**  
4. **Como o orçamento e o realizado evoluem ao longo do tempo?**  
5. **Quais centros de custo apresentam maior eficiência financeira?**  

---

## ⚙️ **FUNCIONALIDADES DO DASHBOARD**

O dashboard permite ao usuário:

- 📅 *Filtrar por departamento (dropdown)*  
- 📊 *Visualizar KPIs financeiros consolidados*  
- 📈 *Acompanhar evolução mensal do orçamento vs realizado*  
- 🎯 *Analisar desempenho por centro de custo*  
- 🔄 *Controlar interação entre visuais (filtros seletivos)*  

> 💡 *Foco em análise rápida de desvios orçamentários e tomada de decisão.*

---

## 📊 **VISUAIS DESENVOLVIDOS**

- 📌 KPI Valor Orçado  
- 📌 KPI Valor Realizado  
- 📌 KPI Saldo  
- 🎯 Gauge de Aderência ao Orçamento  
- 📊 Colunas por Departamento (comparativo)  
- 🍩 Gráfico de Rosca (Orçado vs Realizado)  
- 📈 Linha temporal (evolução mensal)  
- 📊 Barras empilhadas (Orçado x Realizado x Saldo)  
- 🎯 Filtro por Departamento  

---

## 🔄 **PROCESSO DE TRANSFORMAÇÃO DE DADOS (POWER QUERY)**

Principais etapas de ETL:

- 🧹 **Padronização das bases:** Estruturação das tabelas de orçamento e realizado  
- 🔢 **Tipificação de dados:** Ajuste de valores monetários e datas  
- 🔗 **Relacionamento:** Conexão entre tabelas via centro de custo  

> 💡 Processo automatizado para atualização contínua dos dados.

---

## 🧠 **MODELAGEM E CÁLCULOS (DAX)**

### 📌 Modelo de Dados
- Estrutura baseada em **relacionamento entre tabelas de orçamento e realizado**

---

### 📌 Medidas Principais

```DAX id="orcamento-dax-1"
Orçado = SUM(Orcamento[Valor])

Realizado = SUM(Realizado[Valor])

Saldo = [Orçado] - [Realizado]
