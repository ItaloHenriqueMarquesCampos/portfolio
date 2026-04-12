# 📊 **DASHBOARD FINANCEIRO NO POWER BI**

<p align="center">
  <i>Construção de um dashboard financeiro automatizado no Power BI, com foco em análise de receitas, custos e lucro para tomada de decisão estratégica.</i>
</p>

---

![WhatsApp Image 2026-04-11 at 17 02 20](https://github.com/user-attachments/assets/48024f79-987d-4b6b-ad98-c991e62a2e7a)


---

## 🚀 **VISÃO GERAL**

Neste projeto foi desenvolvido um *Dashboard Financeiro completo no Power BI*, utilizando dados provenientes de uma base em *Excel*, com tratamento realizado no *Power Query*.

O objetivo é eliminar processos manuais repetitivos, automatizando a análise financeira. Com isso, ao atualizar a base de dados, basta clicar em *Atualizar* para que todo o dashboard seja recalculado automaticamente.

---

## 📂 **FONTE DE DADOS**

- 📄 **Base única:** *Excel*  
  <sub>Dados financeiros contendo receitas, custos e despesas</sub>

---

## 🎯 **OBJETIVO DO DASHBOARD**

Analisar a performance financeira da empresa, com foco em:

- 💰 *Receita*  
- 💸 *Custos*  
- 🧾 *Despesas*  
- 📈 *Lucro*  

---

## ❓ **PERGUNTAS DE NEGÓCIO**

1. **Qual a receita total no período analisado?**  
2. **Qual o total de custos e despesas?**  
3. **Qual o lucro líquido da operação?**  
4. **Quais categorias geram mais receita?**  
5. **Quais clientes mais contribuem para o faturamento?**  
6. **Como receita, custos e despesas evoluem ao longo do tempo?**  
7. **Existe variação significativa entre meses/anos?**  

---

## ⚙️ **FUNCIONALIDADES DO DASHBOARD**

O dashboard permite ao usuário:

- 📅 *Filtrar por ano (dropdown)*  
- 📊 *Visualizar KPIs financeiros consolidados*  
- 📈 *Analisar evolução temporal (receita, custos e despesas)*  
- 📦 *Explorar receita por categoria*  
- 👥 *Analisar receita por cliente*  

> 💡 *Dashboard totalmente automatizado: atualização com apenas um clique.*

---

## 📊 **VISUAIS DESENVOLVIDOS**

- 📌 KPI Receita  
- 📌 KPI Custo  
- 📌 KPI Despesa  
- 📌 KPI Lucro  
- 🍩 Receita por Categoria (gráfico de rosca)  
- 📈 Receita por Mês/Ano (linha/área)  
- 📊 Receita por Cliente (barras horizontais)  
- 📉 Custos e Despesas (colunas empilhadas)  
- 🎯 Filtro de Ano (segmentação dropdown)  

---

## 🔄 **PROCESSO DE TRANSFORMAÇÃO DE DADOS**

Os dados foram tratados utilizando *Power Query*, com etapas como:

- Definição de tipos de dados  
- Tratamento de inconsistências  
- Padronização de colunas  
- Criação de regras automatizadas de limpeza  

> 💡 Todas as transformações são reaplicadas automaticamente a cada atualização.

---

## 🧠 **MODELAGEM E CÁLCULOS (DAX)**

Foi criada uma coluna calculada para viabilizar o cálculo do lucro:

```DAX
Valor com Sinal = IF(Movimentação[Tipo] = "Saída", -Movimentação[Valor], Movimentação[Valor])
