# 🔷 DCF Valuation Model — Nubank (H1 2025)

## 📊 Visão Geral

Análise técnica integrada de uma Demonstração de Fluxo de Caixa de instituição 
financeira brasileira com objetivo de construir um modelo de valuation por DCF 
(Discounted Cash Flow).

**Dados Base:** Demonstrações Contábeis do Nubank — Semestre findo 30/06/2025

**Status:** ✅ Concluído | **Última Atualização:** Junho 2026

---

## 🎯 Objetivo

Estimar o **valor intrínseco** do Nubank através de:
1. Análise aprofundada de fluxo de caixa histórico
2. Projeção de fluxos futuros (5 anos)
3. Cálculo de WACC (Weighted Average Cost of Capital)
4. Análise de sensibilidade em múltiplos cenários

---

## 📈 Principais Descobertas

| Métrica | Valor | Interpretação |
|---------|-------|----------------|
| **FCFF Operacional** | R$ 2,9B | Instituição gera caixa forte |
| **Provisão/Crédito Bruto** | 35,0% | Cobertura de risco adequada |
| **Crescimento Projetado (5Y)** | 8-12% | Cenário conservador a otimista |
| **Valor Intrínseco** | *[será calculado]* | Resultado da análise DCF |

---

## 🛠️ Ferramentas & Tecnologias

- **Excel**: Modelagem principal, sensibilidade, projeções
- **Python 3.8+**: Validação de dados, automação
  - `pandas`: Manipulação de dados
  - `numpy`: Cálculos numéricos
  - `matplotlib` / `seaborn`: Visualizações
- **Power BI**: Dashboard de KPIs
- **Bloomberg Terminal**: Pesquisa de comparáveis

---

## 📂 Estrutura do Projeto
dcf-nubank-valuation/ │ ├── DCF_Nubank_Model.xlsx # Modelo principal ├── data/ │ ├── nubank_statements.csv # Dados brutos extraídos │ └── assumptions.csv # Premissas do modelo │ ├── src/ │ ├── data_extraction.py # Script para extrair dados │ ├── dcf_model.py # Cálculos DCF │ ├── sensitivity_analysis.py # Análise de cenários │ └── visualization.py # Gráficos e dashboards │ ├── outputs/ │ ├── dcf_summary.png # Gráfico resumo │ ├── sensitivity_heatmap.png # Heat map de sensibilidade │ └── valuation_report.pdf # Relatório executivo │ └── requirements.txt # Dependências Python

