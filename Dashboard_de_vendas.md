# 🛍️ **DASHBOARD ANALÍTICO DE VENDAS (PINSK)**

<p align="center">
  <i>Análise de desempenho comercial no varejo de moda masculina com foco em receita, margem e performance de vendedores.</i>
</p>

---

![WhatsApp Image 2026-04-11 at 16 58 34](https://github.com/user-attachments/assets/0d3cee67-6a13-4414-911c-9255befc3421)


---

## 🚀 **VISÃO GERAL**

Neste projeto foi desenvolvido um *Dashboard de Vendas completo no Power BI* para a loja **PINSK**, do segmento de varejo de moda masculina.

Os dados foram extraídos de uma base em *Excel* e tratados no *Power Query*, com o objetivo de automatizar o processo comercial e eliminar rotinas manuais repetitivas, como downloads constantes de planilhas e manipulações inconsistentes de dados.

---

## 📂 **FONTE DE DADOS**

- 📄 **Base única:** *Excel* (dividida em 3 abas)

### 📊 Estrutura dos dados:

- **Tabela Fato:**  
  - Registro de vendas (notas fiscais, quantidades, receitas, custos e códigos)

- **Tabelas Dimensão:**  
  - Cadastro de Produtos (características e imagens)  
  - Cadastro de Vendedores (nomes e fotos)

---

## 🎯 **OBJETIVO DO DASHBOARD**

Analisar a performance comercial da empresa com foco em:

- 💰 *Receita Líquida*  
- 💸 *Custos*  
- 📈 *Margem Bruta*  
- 🛍️ *Quantidade de Vendas*  

---

## ❓ **PERGUNTAS DE NEGÓCIO**

1. **Qual o total de receita, custo e margem no período analisado?**  
2. **Qual o volume total de vendas (notas fiscais distintas)?**  
3. **Qual o ranking de performance dos vendedores?**  
4. **Quais produtos mais contribuem para o resultado?**  
5. **Como as métricas evoluem ao longo do tempo?**  

---

## ⚙️ **FUNCIONALIDADES DO DASHBOARD**

O dashboard permite ao usuário:

- 📅 *Filtrar por Ano e Gerente (dropdown)*  
- 📊 *Visualizar KPIs comerciais consolidados*  
- 🎛️ *Alternar métricas dinamicamente (Receita, Margem e Vendas)*  
- 🔍 *Explorar detalhes via Tooltip com imagem do produto*  
- 👥 *Analisar ranking de vendedores com imagens*  

> 💡 *Alta interatividade e análise dinâmica com poucos cliques.*

---

## 📊 **VISUAIS DESENVOLVIDOS**

- 📌 KPI Receita Líquida  
- 📌 KPI Custo Total  
- 📌 KPI Margem Bruta  
- 📌 KPI Quantidade de Vendas  
- 📊 Métricas por Produto (barras dinâmicas)  
- 📈 Métricas por Ano/Mês (linha dinâmica)  
- 📋 Ranking de Vendedores (tabela com imagens)  
- 🎯 Filtros (Ano e Gerente)  
- 🖼️ Tooltip customizado com imagem do produto  

---

## 🔄 **PROCESSO DE TRANSFORMAÇÃO DE DADOS (POWER QUERY)**

Principais etapas de ETL:

- 💰 **Tipagem financeira:** Receita e Custo como moeda (decimal fixo)  
- 🧹 **Limpeza de dados:** Remoção de colunas desnecessárias (ex: Receita Bruta)  
- 🔤 **Padronização:** Nota Fiscal mantida como texto  
- 🔗 **Validação de chaves:** Garantia de integridade entre tabelas (produto e vendedor)  

> 💡 Processo automatizado e reaplicável a cada atualização.

---

## 🧠 **MODELAGEM E CÁLCULOS (DAX)**

### 📌 Modelo de Dados
- Estrutura em **Star Schema** (Fato + Dimensões)

---

### 📌 Tabela Calendário

```DAX
Calendario = CALENDARAUTO()
