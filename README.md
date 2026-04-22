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


---

## 🚀 Como Executar

### 1. Clonar o Repositório
bash
git clone https://github.com/marcelomourafreire/dcf-nubank-valuation.git
cd dcf-nubank-valuation

2. Instalar Dependências
bash

pip install -r requirements.txt

3. Executar a Análise
bash

python src/data_extraction.py
python src/dcf_model.py
python src/sensitivity_analysis.py
python src/visualization.py

4. Visualizar Resultados

    Abrir DCF_Nubank_Model.xlsx para ver o modelo completo
    Abrir outputs/dcf_summary.png para resumo visual
    Abrir outputs/valuation_report.pdf para relatório completo

📊 Modelo DCF — Resumo Técnico
Premissas Principais
Premissa 	Valor 	Fonte/Justificativa
Revenue Growth (5Y) 	8-12% 	Histírico de crescimento do setor
WACC 	8,5% 	Beta setorial + custo de dívida
Terminal Growth 	3,0% 	Crescimento perpetual conservador
CAPEX/Receita 	2-3% 	Típico para instituições digitais
Estrutura de Cálculo

    Receitas Projetadas: Baseadas em crescimento histórico + cenários econômicos
    EBIT Operacional: Ajustado por provisões de crédito esperadas
    FCFF: EBIT × (1 - Tax Rate) + Ajustes Não-Caixa - CAPEX - Variação de Capital de Giro
    Valor Terminal: FCFF(ano 5) × (1 + g) / (WACC - g)
    Valor Presente: ∑ FCFF(t) / (1 + WACC)^t + Valor Terminal / (1 + WACC)^5

📈 Resultados da Análise de Sensibilidade
WACC ↓ / Crescimento → 	6% 	8% 	10% 	12%
7,5% 	Alto 	Otimista 	Muito Otimista 	Extremo
8,5% 	Moderado 	Base (Recomendado) 	Moderado Alto 	Otimista
9,5% 	Baixo 	Conservador 	Moderado 	Base Alt

(Valores de valuation em BRL bilhões — valores numéricos a completar na análise)
🔍 Principais Drivers Analisados
Fluxo de Caixa (H1 2025)
Atividade 	Valor (R$ bilhões) 	Impacto
Operações de Crédito 	-42,1 	Reestruturação/amortização acelerada
Depósitos Captados 	+8,2 	Crescimento da base de clientes
Depósitos Compulsórios 	-1,6 	Pressão regulatória esperada
FCFF Operacional 	+2,9 	Geração de caixa positiva ✅
📌 Limitações & Considerações

⚠️ Importante: Este projeto é educacional e para fins de análise técnica.

    Baseado apenas em dados públicos (Demonstrações Contábeis)
    Premissas sujeitas a revisão com novas informações de mercado
    Não constitui recomendação de investimento
    Cenários macro podem mudar rapidamente

🤝 Contribuições

Este projeto é pessoal/educacional. Feedback é bem-vindo!
📧 Contato

    Email: ma.mo.fr@gmail.com
    LinkedIn: linkedin.com/in/marcelomourafreire
    GitHub: @marcelomourafreire

📜 Licença

MIT License — Veja LICENSE para detalhes

