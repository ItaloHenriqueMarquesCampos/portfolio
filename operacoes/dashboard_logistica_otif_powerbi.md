# 🚚 **DASHBOARD ANALÍTICO DE LOGÍSTICA (OTIF)**

<p align="center">
  <i>Análise de desempenho logístico com foco em entregas no prazo, completude e identificação de falhas operacionais.</i>
</p>

---

![WhatsApp Image 2026-04-11 at 17 00 39](https://github.com/user-attachments/assets/e57dae89-0503-448d-810d-5794e201955d)


---

## 🚀 **VISÃO GERAL**

Neste projeto foi desenvolvido um *Dashboard de Logística completo no Power BI*, utilizando dados provenientes de uma base em *Excel*, com extração e tratamento realizados no *Power Query*.

O objetivo é automatizar a análise de desempenho de entregas e problemas logísticos da empresa **Elo X Transportes e Logística**, eliminando processos manuais. Com isso, ao atualizar a base de dados, todos os indicadores e gráficos são recalculados automaticamente.

---

## 📂 **FONTE DE DADOS**

- 📄 **Base única:** *Excel*  
  <sub>Arquivo extraído de sistema e importado para o Power BI</sub>

- 📦 **Dados contemplados:**
  - Pedidos  
  - Destinos  
  - Datas previstas e realizadas  
  - Tipos de veículos  
  - Filiais  
  - Ocorrências e devoluções  

---

## 🎯 **OBJETIVO DO DASHBOARD**

Analisar a performance da operação logística com foco nos principais indicadores:

- ⏳ **On Time:** Entregas realizadas dentro do prazo  
- 📦 **In Full:** Entregas completas, sem falhas  
- 🎯 **OTIF (On Time In Full):** Indicador consolidado de qualidade logística  
- ⚠️ **Ocorrências:** Falhas, devoluções e problemas operacionais  

---

## ❓ **PERGUNTAS DE NEGÓCIO**

Este dashboard responde às seguintes questões estratégicas:

1. **Qual filial está impactando negativamente o OTIF?**  
2. **Existe algum setor responsável pela maior parte das ocorrências?**  
3. **Qual o principal motivo de falhas nas entregas?**  
4. **Como o OTIF evolui ao longo do tempo?**  
5. **Onde as ocorrências estão concentradas geograficamente?**  

---

## ⚙️ **FUNCIONALIDADES DO DASHBOARD**

O dashboard permite ao usuário:

- 📅 *Filtrar por Ano, Mês e Filial (dropdown com busca)*  
- 📊 *Visualizar KPIs percentuais com gráficos dinâmicos*  
- 📈 *Analisar evolução temporal do OTIF*  
- 🏢 *Identificar alertas por filial com formatação condicional*  
- 🗺️ *Visualizar ocorrências em mapa interativo*  
- 🎨 *Personalizar visual (cores, temas e layout)*  

> 💡 *Facilitando análises rápidas e decisões operacionais mais assertivas.*

---

## 📊 **VISUAIS DESENVOLVIDOS**

- 🍩 KPIs (% OTIF, % On Time, % In Full) — gráficos de rosca  
- 📈 % OTIF por Ano/Mês — gráfico de área  
- 📊 Ocorrências por Responsável — barras clusterizadas  
- 📊 Ocorrências por Motivo — barras ajustadas para textos longos  
- 🗺️ Ocorrências por Estado e Cidade — mapa dinâmico (Azure Maps)  
- 📋 Visão por Filial — matriz com indicadores e alertas visuais  
- 🎯 Filtros — segmentações interativas (Ano, Mês, Filial)  

---

## 🔄 **PROCESSO DE TRANSFORMAÇÃO DE DADOS (POWER QUERY)**

Principais etapas de ETL aplicadas:

- 🧹 **Limpeza inicial:** Remoção de linhas desnecessárias e ajuste de cabeçalhos  
- 🔢 **Tipificação:** Definição correta de tipos de dados  
- 🔄 **Substituição de valores:** Padronização de inconsistências  
- ✂️ **Divisão de colunas:** Extração de Região, Estado e Cidade a partir de dados compostos  

> 💡 Todas as etapas são automatizadas e reaplicadas a cada atualização.

---

## 🧠 **MODELAGEM E CÁLCULOS (DAX)**

### 📌 Coluna Calculada

```DAX
On Time = IF('Pedidos'[Data da entrega] <= 'Pedidos'[Data prevista] && 'Pedidos'[Data da entrega] <> BLANK(), "sim", "não")
