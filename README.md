# Projeto de Análise de Risco de Crédito — German Credit Dataset

## Status do Projeto

**Em desenvolvimento** — fase de entendimento dos dados, documentação e análise exploratória.

Este repositório apresenta um projeto de **Análise de Risco de Crédito**, utilizando o clássico **German Credit Dataset**, amplamente usado em estudos acadêmicos e aplicações de Machine Learning no setor financeiro.

Neste momento, o foco do projeto está em:

* Compreensão do problema de negócio
* Organização e documentação dos dados
* Análise Exploratória de Dados (EDA)

As etapas de **modelagem preditiva e avaliação** serão desenvolvidas posteriormente.

---

## Objetivo do Projeto

O objetivo é analisar o perfil de clientes solicitantes de crédito e identificar padrões associados ao **risco de inadimplência**, apoiando decisões de concessão de crédito.

Ao final do projeto, será desenvolvido um **modelo de classificação** capaz de prever se um cliente representa **bom ou mau risco de crédito**, com base em características financeiras, pessoais e comportamentais.

---

## Contexto de Negócio

Instituições financeiras precisam equilibrar dois fatores críticos:

* **Redução do risco de inadimplência**
* **Manutenção da concessão de crédito de forma sustentável**

Uma análise inadequada pode gerar perdas financeiras, enquanto critérios excessivamente restritivos podem reduzir oportunidades de negócio. Este projeto simula esse cenário, utilizando dados históricos para apoiar decisões mais eficientes.

---

## Dataset Utilizado

* **Nome:** German Credit Dataset
* **Origem:** UCI Machine Learning Repository
* **Registros:** 1000 clientes
* **Variáveis:** 20 preditoras + 1 variável alvo

O dataset contém variáveis **numéricas e categóricas**, representadas originalmente por códigos alfanuméricos.

A descrição detalhada das variáveis pode ser encontrada no **[Dicionário de Dados](docs/data_dictionary.md)**.

---

## Etapas do Projeto

1. Entendimento do problema
2. Organização do repositório
3. Documentação dos dados
4. Análise Exploratória de Dados (EDA)
5. Pré-processamento *(em breve)*
6. Modelagem preditiva *(em breve)*
7. Avaliação dos modelos *(em breve)*

---

## Estrutura do Repositório

```
credit-risk-german/
│
├── README.md
├── requirements.txt
│
├── data/
│   ├── raw/          # Dados originais e legíveis
│   └── processed/    # Dados tratados para modelagem
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_modeling.ipynb
│   └── 04_evaluation.ipynb
│
├── docs/
│   └── data_dictionary.md
│
└── results/
    └── figures/
```

---

## Tecnologias Utilizadas

* Python
* Pandas
* NumPy
* Matplotlib / Seaborn
* Scikit-learn *(etapas futuras)*

---

## Autora

**Aline Brito Lima**

Cientista de Dados (em transição de carreira)

> Projeto desenvolvido com foco em aprendizado, boas práticas e construção de portfólio profissional.

---

## Próximos Passos

* Finalizar Análise Exploratória de Dados
* Tratar variáveis categóricas
* Implementar modelos de classificação
* Avaliar desempenho com métricas adequadas (AUC, ROC, KS)
