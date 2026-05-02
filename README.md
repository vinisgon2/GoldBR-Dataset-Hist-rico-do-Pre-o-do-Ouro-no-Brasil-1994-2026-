# GoldBR-Dataset-Hist-rico-do-Pre-o-do-Ouro-no-Brasil-1994-2026-
Este repositório contém o **GoldBR**, um dataset histórico do preço do ouro no Brasil, construído a partir de dados do Banco Central do Brasil (fonte Refinitiv), abrangendo o período de **1994 a 2026**.
O objetivo deste projeto é fornecer uma base estruturada, reprodutível e pronta para uso em pesquisas de:
- Ciência de Dados
- Séries Temporais
- Finanças Quantitativas
- Modelagem Preditiva

---

## 📊 Sobre o Dataset

O dataset contém dados históricos do **ouro tipo A (24K)** no mercado brasileiro, incluindo valores mínimos de compra e venda.

Os dados foram:
- Coletados
- Tratados
- Padronizados
- Agregados (mensalmente)
- Enriquecidos com variáveis derivadas

---

## 📁 Estrutura do Repositório

GoldBR/
│
├── data/
│ ├── gold_raw.csv
│ ├── gold_processed.csv
│
├── notebooks/
│ ├── analise_ouro.ipynb
│
├── src/
│ ├── processamento.py
│
├── images/
│ ├── serie_temporal.png
│ ├── variacao_mensal.png
│
├── README.md


---

## 🧾 Dicionário de Dados

| Campo        | Tipo     | Descrição |
|-------------|----------|----------|
| Data        | Data     | Data da cotação |
| Tipo        | Texto    | Tipo do ouro (A – 24K) |
| Compra      | Numérico | Valor mínimo de compra |
| Venda       | Numérico | Valor mínimo de venda |
| Resultado%  | Numérico | Variação percentual mensal |
| Mês         | Inteiro  | Mês da observação (1–12) |
| Ano         | Inteiro  | Ano da observação |
| No.Mes      | Texto    | Mês formatado (01–12) |

---

## ⚙️ Metodologia

### 1. Coleta
Dados obtidos via Banco Central do Brasil (fonte Refinitiv).

### 2. Pré-processamento
- Limpeza de dados
- Padronização de datas
- Ordenação temporal

### 3. Agregação
Conversão de dados diários para frequência mensal.

### 4. Enriquecimento

Cálculo da variação percentual:

```math
Resultado\% = \frac{Preço_t - Preço_{t-1}}{Preço_{t-1}} \times 100
📈 Principais Características do Dataset
Série histórica longa (1994–2026)

Presença de não estacionariedade

Evidência de clusterização de volatilidade

Indícios de sazonalidade

Influência de mudanças estruturais econômicas

🔍 Possíveis Aplicações
Este dataset pode ser utilizado para:

Modelagem de séries temporais (ARIMA, GARCH)

Machine Learning e Deep Learning

Estratégias quantitativas

Análise de risco

Estudos econômicos

Backtesting de estratégias financeiras

▶️ Como Reproduzir
Requisitos
Python 3.10+
pandas
numpy
matplotlib
seaborn
Execução
git clone https://github.com/seu-usuario/goldbr.git
cd goldbr
pip install -r requirements.txt
jupyter notebook
Execute o notebook:

notebooks/analise_ouro.ipynb
📊 Exemplos de Análise
O notebook inclui:

Série temporal do preço do ouro

Variação percentual mensal

Identificação de padrões

Análise por período (1994–2026 vs 2016–2026)

⚠️ Limitações
Dependência de fonte secundária (Refinitiv)

Possíveis lacunas em períodos antigos

Não inclui variáveis macroeconômicas (ex: inflação, câmbio)

Mudanças estruturais podem afetar análises preditivas

📦 Disponibilização
O dataset está disponível neste repositório em formato:

CSV (dados brutos e processados)

📄 Citação
Se utilizar este dataset, cite:

GONÇALVES, Vinícius S. GoldBR: Dataset Histórico do Preço do Ouro no Brasil (1994–2026), 2026.
📜 Licença
Este projeto é disponibilizado para uso acadêmico e educacional.

👨‍💻 Autor
Vinícius Silva Gonçalves
Mestrando em Ciência da Computação

⭐ Contribuição
Contribuições são bem-vindas via pull requests.


---

# 🔥 O QUE ESSE README FAZ POR VOCÊ

Ele cobre exatamente o que avaliadores do DSW procuram:

✔ Documentação clara  
✔ Reprodutibilidade  
✔ Estrutura de dados  
✔ Aplicabilidade  
✔ Limitações (muito importante)  

---

# 🚀 SE QUISER IR ALÉM (RECOMENDADO)

Posso te ajudar a:

- gerar automaticamente o `requirements.txt`
- criar gráficos para colocar na pasta `/images`
- escrever a descrição do repositório otimizada (GitHub + artigo)

Só falar 👍
