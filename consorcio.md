# 📊 Painel de Comissionamento de Vendas – Consórcio

**Desenvolvimento de uma solução completa para automatizar o cálculo de comissões, otimizar a gestão de vendas e facilitar a visualização de resultados em empresas do setor de consórcios.**

---

## 🔧 Tecnologias Utilizadas

- 📄 **Google Sheets** – Estruturação dos dados e lógica de cálculo
- 📊 **Looker Studio** – Visualização de resultados por meio de dashboards interativos
- 🧠 **Fórmulas avançadas** – `SE`, `SOMASES`, `PROCV`, `LET`, `CORRESP`, `COL`, `SEERRO`, entre outras
- ⏱️ **Atualização automática** – A cada 15 minutos via Google Sheets

---

## 🎯 Objetivos do Projeto

- Automatizar o controle de comissões por **vendedor**, **gestor** e para a **empresa**
- Facilitar o acompanhamento mensal de parcelas comissionadas
- Reduzir erros manuais no cálculo e controle de metas
- Fornecer visualizações amigáveis e exportáveis

---

## ⚙️ Funcionalidades

### 📋 Estrutura da Planilha

- Cálculo automático baseado em:
  - Mês da venda (`L`)
  - Nível do vendedor (`Q`)
  - Segmento (Imóvel ou Automóvel) (`F`)
  - Base de cálculo (`N`)
- Controle das **parcelas** comissionadas de acordo com o mês da venda
- Fórmulas robustas com tratamento de erros e valores nulos
- Comissões adaptáveis de 1ª a 18ª parcela por perfil

### 📊 Painel no Looker Studio

- Filtros por:
  - Nome do vendedor
  - Mês
  - Tipo de produto
  - Status da venda
- Atualização a cada 15 minutos
- Exportação para PDF ou Google Sheets
- Relatórios segmentáveis para gestão individual

---

## 🧠 Destaques Técnicos

```excel
=SEERRO(
  SE(
    E(
      COL() - COL($V$2) + 1 >= CORRESP($L3; {"Janeiro";"Fevereiro";...}; 0);
      ÉNÚM(PROCV($U3; ...));
      $P3 > 0
    );
    PROCV(...) * $P3;
    ""
  );
  ""
)
