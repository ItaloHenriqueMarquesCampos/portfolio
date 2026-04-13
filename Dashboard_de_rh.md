# 👥 **DASHBOARD ANALÍTICO DE RECURSOS HUMANOS (HEADCOUNT & COMPETÊNCIAS)**

---

![rh](https://github.com/user-attachments/assets/0bc527d1-0b29-479d-b3a7-c1bdb5b87f7f)

---

## 🚀 **VISÃO GERAL**

Neste projeto foi desenvolvido um *Dashboard de RH no Power BI*, utilizando dados provenientes de uma base em *Excel*, com tratamento e modelagem realizados no *Power Query*.

O objetivo é automatizar a análise do quadro de funcionários ao longo do tempo, além de comparar o desempenho individual com a média geral da empresa.

---

## 📂 **FONTE DE DADOS**

- 📄 **Base principal:** *Excel (Cadastro de Funcionários)*  

### 📊 Estrutura dos dados:

- Matrícula (ID RH)  
- Nome  
- Data de Contratação  
- Data de Demissão  
- Cargo  
- Competências:  
  - Trabalho em Equipe  
  - Liderança  
  - Comunicação  
  - Iniciativa  
  - Organização  

- 📅 **Tabela Auxiliar:**  
  - Calendário (2010 a 2018)

---

## 🎯 **OBJETIVO DO DASHBOARD**

Analisar a área de Recursos Humanos com foco em:

- 👥 *Headcount (funcionários ativos)*  
- 📈 *Turnover (contratações e demissões)*  
- ⭐ *Desempenho por competências*  
- 📊 *Comparativo entre colaborador e média da empresa*  

---

## ❓ **PERGUNTAS DE NEGÓCIO**

1. **Quantos funcionários ativos existem ao longo dos anos?**  
2. **Quantas contratações e demissões ocorreram no período?**  
3. **Qual o desempenho individual por competência?**  
4. **O colaborador está acima ou abaixo da média da empresa?**  

---

## ⚙️ **FUNCIONALIDADES DO DASHBOARD**

O dashboard permite ao usuário:

- 📅 *Analisar evolução do headcount ao longo dos anos*  
- 👤 *Filtrar por funcionário (dropdown com busca)*  
- 📊 *Comparar desempenho individual vs média global*  
- 🔍 *Visualizar indicadores sem interferência de filtros específicos*  

> 💡 *Facilitando análises estratégicas de pessoas e desempenho.*

---

## 📊 **VISUAIS DESENVOLVIDOS**

- 🕸️ Competências do Funcionário (Gráfico de Radar)  
- 📋 Headcount ao longo do tempo (Matriz)  
- 📈 Indicadores de contratação e demissão  
- 🎯 Filtro por Funcionário (dropdown com busca)  

---

## 🔄 **PROCESSO DE TRANSFORMAÇÃO DE DADOS (POWER QUERY)**

Principais etapas de ETL:

- 🔁 **Duplicação da base:** Criação da tabela de competências  
- 🧹 **Limpeza de dados:** Remoção de colunas irrelevantes  
- 🔄 **Unpivot (colunas → linhas):**  
  Transformação das competências em formato analítico  

> 💡 Estrutura ideal para análises dinâmicas e visuais avançados.

---

## 🧠 **MODELAGEM E CÁLCULOS (DAX)**

### 📌 Modelo de Dados
- Estrutura com **tabela fato + tabela calendário + tabela de competências**

---

### 📌 Média Global (Ignorando Filtros)

```DAX id="rh-dax-1"
Media Notas = 
CALCULATE(
    AVERAGE(Competencias[Nota]),
    ALL(Competencias)
)
