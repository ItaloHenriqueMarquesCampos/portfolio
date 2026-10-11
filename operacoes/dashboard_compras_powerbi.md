# 🛒 **DASHBOARD ANALÍTICO DE COMPRAS**

---

![WhatsApp Image 2026-04-13 at 19 28 14](https://github.com/user-attachments/assets/ed82c6fc-531a-4aff-8ae9-c6067f2a2394)

---

## 🚀 **VISÃO GERAL**

Neste projeto foi desenvolvido um *Dashboard completo de Compras no Power BI*, criado a partir de uma base em *Excel*, com extração e tratamento realizados no *Power Query*.

O objetivo é automatizar a análise dos principais indicadores do setor de compras, eliminando processos manuais e centralizando as informações em um relatório dinâmico e interativo.

---

## 📂 **FONTE DE DADOS**

- 📄 **Base única:** *Excel*

### 📊 Estrutura dos dados:

- **Tabela Fato:**  
  - Histórico de compras (quantidades, datas, descontos e códigos)

- **Tabelas Dimensão:**  
  - Compradores  
  - Fornecedores  
  - Matérias-primas  

---

## 🎯 **OBJETIVO DO DASHBOARD**

Analisar a performance do setor de compras com foco em:

- 💰 *Custos Totais (com e sem desconto)*  
- 💸 *Saving (economia gerada)*  
- ⏳ *Lead Time (tempo entre pedido e entrega)*  
- ⚠️ *Atrasos de entrega*  

---

## ❓ **PERGUNTAS DE NEGÓCIO**

1. **Qual o custo total efetivo no período?**  
2. **Quanto foi economizado nas negociações?**  
3. **Qual o tempo médio de entrega (Lead Time)?**  
4. **Qual o atraso médio dos fornecedores?**  
5. **Quais fornecedores e compradores têm melhor desempenho?**  
6. **Como custos e savings evoluem ao longo do tempo?**  

---

## ⚙️ **FUNCIONALIDADES DO DASHBOARD**

O dashboard permite ao usuário:

- 📅 *Filtrar por Ano, Fornecedor e Comprador*  
- 📊 *Visualizar KPIs consolidados*  
- 📈 *Acompanhar evolução mensal de custos e savings*  
- 👥 *Analisar performance de fornecedores*  
- 🔍 *Explorar detalhes via Tooltip com mini dashboard*  

> 💡 *Facilitando análises rápidas e decisões mais eficientes.*

---

## 📊 **VISUAIS DESENVOLVIDOS**

- 📌 KPI Custo Total com Desconto  
- 📌 KPI Lead Time de Compra  
- 📌 KPI Atraso Médio  
- 📈 Custo Mensal (gráfico de área)  
- 📈 Saving Mensal (gráfico de área)  
- 📊 Lead Time por Fornecedor (barras horizontais)  
- 📊 Saving por Fornecedor (barras horizontais)  
- 🎯 Filtros interativos (Ano, Fornecedor, Comprador)  

---

## 🔄 **PROCESSO DE TRANSFORMAÇÃO DE DADOS (POWER QUERY)**

Principais etapas de ETL:

- 🧹 **Limpeza de dados:** Remoção de linhas em branco  
- 🔢 **Tipificação:** Ajuste correto de datas, números e textos  
- ⚙️ **Coluna condicional:** Classificação automática de entregas (No prazo / Atrasado)  

> 💡 Processo automatizado e reaplicado a cada atualização.

---

## 🧠 **MODELAGEM E CÁLCULOS (DAX)**

### 📌 Modelo de Dados
- Estrutura em **Star Schema**

---

### 📌 Tabela Calendário

```DAX
dCalendario = CALENDARAUTO()
