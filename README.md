
# 📊 *Dashboard de Performance Comercial*  
### *Otimizando Decisões com Análise de Dados*

## 👨‍💼 Autor  
**Italo Henrique Marques Campos**

## 🎯 Objetivo do Projeto  
Desenvolver um dashboard interativo e estratégico, com base em análise de dados, para melhorar o desempenho comercial, a gestão de leads e a tomada de decisões dentro de uma organização educacional.

---

## 🏢 Contexto da Empresa  
A *Empresa X Educação* é uma instituição privada com mais de 100 colaboradores na área comercial. Atua com diversos tipos de cursos (graduação, pós, extensão, técnico, EJA).  

O principal desafio: **informações comerciais fragmentadas** em diversas planilhas do Google Sheets, conectadas via `IMPORTRANGE`, dificultando análise de desempenho, controle de leads e decisões gerenciais.

---

## 🚨 Problema Identificado  
A visualização e a interpretação de dados de vendas e leads eram ineficientes, dificultando decisões estratégicas. Faltava centralização e padronização das informações, o que levava a uma gestão reativa e perda de oportunidades.

---

## 💡 Solução Proposta  
Implementação de um **dashboard no Looker Studio**, com consolidação das informações em uma planilha mestra (data warehouse), permitindo:

- Monitoramento de desempenho individual e por equipe  
- Análise de leads recebidos, convertidos e perdidos  
- Acompanhamento de gincanas de vendas  
- Identificação de gargalos e oportunidades  

---

## 🔄 Metodologia  
Baseada no ciclo **PDCA (Plan-Do-Check-Act)**:

### 📌 *Plan – Planejar*  
- Identificação do problema  
- Definição de objetivos e KPIs  
- Mapeamento das fontes de dados  
- Estrutura do dashboard planejada

### ⚙️ *Do – Executar*  
- Consolidação dos dados de +100 vendedores em uma planilha mestra  
- Extração para o Looker Studio via Google Sheets  
- Modelagem dos dados (dimensões e métricas)  
- Criação dos dashboards interativos

### 📈 *Check – Verificar*  
- Validação dos resultados apresentados  
- Testes de filtros, gráficos e tabelas  
- Identificação de melhorias e correções

### 🔁 *Act – Agir*  
- Proposição de decisões estratégicas com base nos insights  
- Padronização de práticas eficazes  
- Planejamento contínuo para evolução do dashboard

---

## 🧱 Etapas do Projeto

### 🔹 1. Coleta e Integração de Dados  
- Planilhas de vendas individuais → planilha mestra (Data Warehouse)  
- Dados: vendas, leads, desempenho anual, gincanas

### 🔹 2. Modelagem de Dados  
- **Dimensões:** vendedor, equipe, modalidade, origem do lead, mês  
- **Métricas:** vendas, leads recebidos, leads perdidos, ticket médio, faturamento

### 🔹 3. Desenvolvimento dos Dashboards

#### 📌 Relatório de Vendas  
- Quantidade de vendas e alunos  
- Faturamento total  
- Vendas por modalidade, faculdade, origem  
- Tabelas por vendedor e por equipe  
- Segmentação por forma de pagamento e status do colaborador  

#### 📌 Relatório de Desempenho Anual  
- Faturamento mensal (total e à vista)  
- Desempenho por equipe e por colaborador  
- Comparativo por mês

#### 📌 Relatório de Leads  
- Leads recebidos, perdidos, com venda direta  
- Origem, horário de distribuição, certificadora  
- Motivos de desqualificação  

#### 📌 Relatório de Gincanas de Vendas  
- Metas por equipe e colaborador  
- Valor atingido vs. esperado  
- Ranking e engajamento

### 🔹 4. Controles Interativos  
- Filtros por mês, vendedor, equipe, curso, origem, status do lead  
- Segmentações para análises dinâmicas e drill-down

### 🔹 5. Análise e Interpretação  
- Exploração dos dados  
- Identificação de padrões, gargalos e oportunidades  

### 🔹 6. Proposição de Decisões Estratégicas  
- Recomendações com base nos KPIs  
- Exemplos de decisões sugeridas:

```markdown
📌 Taxa de Conversão por Origem
→ Aumentar investimento em origens com alta conversão
→ Rever estratégias em origens com baixa performance

📌 Faturamento Médio por Vendedor
→ Treinamentos para vendedores com baixo desempenho
→ Compartilhamento de boas práticas de top performers
```

---

## 📚 Disciplinas Aplicadas (do curso de pós-graduação)

- **Arquitetura Big Data:** estruturação de dados em larga escala  
- **Arquitetura de Dados:** organização do Data Warehouse  
- **Business Intelligence and Analytics:** uso do Looker Studio para decisões  
- **Ética na Era Digital:** tratamento responsável dos dados (LGPD)

---

## 📌 Plano de Ação 5W2H (resumido)

| **O quê (What)**                       | **Por quê (Why)**                                   | **Quem (Who)**             | **Como (How)**                              |
|---------------------------------------|-----------------------------------------------------|-----------------------------|----------------------------------------------|
| Consolidar planilhas em data warehouse | Padronizar e centralizar dados                     | Analista de Dados           | ETL com Google Sheets + Looker Studio        |
| Criar dashboards segmentados          | Facilitar análises estratégicas                    | Analista + Gestão Comercial | Visualizações com filtros dinâmicos          |
| Validar consistência dos dados        | Garantir confiabilidade dos indicadores             | Analista de Dados           | Testes de valores, nulos, duplicidade        |
| Gerar insights e decisões             | Apoiar a gestão com dados acionáveis                | Analista + Gestores         | Apresentação de relatórios e recomendações   |

---

## ✅ Resultados Esperados

- Redução do tempo de análise e tomada de decisão  
- Aumento do desempenho individual e por equipe  
- Melhor gestão de leads e aproveitamento de campanhas  
- Visibilidade clara e centralizada do funil de vendas
