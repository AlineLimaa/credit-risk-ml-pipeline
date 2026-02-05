# Modelagem de Risco de Crédito

Este repositório apresenta um projeto completo de **Ciência de Dados aplicada ao risco de crédito**, utilizando a base **German Credit Data**. O projeto foi estruturado com foco em **clareza, reprodutibilidade, boas práticas de modelagem** e **comunicação com públicos técnicos e não técnicos**, simulando um fluxo próximo ao utilizado em ambientes profissionais.

O objetivo é desenvolver e avaliar modelos de **classificação binária**, capazes de prever se um cliente representa **bom ou mau risco de crédito**, considerando os desafios típicos desse tipo de problema, como desbalanceamento de classes e necessidade de interpretabilidade.

---

## Visão Geral do Pipeline

O projeto foi organizado em **notebooks sequenciais**, onde cada etapa depende da anterior, formando um **pipeline lógico e reprodutível**, conforme descrito abaixo:

1. Ingestão e análise inicial dos dados
2. Exploração e análise de dados (EDA)
3. Feature engineering e preparação dos dados
4. Modelagem e avaliação dos modelos

Cada notebook possui um escopo bem definido e não realiza etapas que pertencem a fases posteriores, evitando vazamento de dados e garantindo separação de responsabilidades.

---

## Estrutura do Repositório

````text
├── src/
├── notebooks/
│   ├── 01_ingestao_e_analise_inicial.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_preprocessamento.ipynb
│   └── 04_modelagem.ipynb
│
├── models/
├── docs/
├── data/
├── requirements.txt
└── README.md
```text
├── notebooks/
│   ├── 01_ingestao_e_analise_inicial.ipynb
│   ├── 02_eda.ipynb
│   ├── 03_preprocessamento.ipynb
│   └── 04_modelagem.ipynb
│
├── data/
│   ├── raw/
│   └── processed/
│
├── artifacts/
│   └── preprocessador.joblib
│
└── README.md
````

---

## Descrição dos Notebooks

### Notebook 1 – Ingestão e Análise Inicial dos Dados

Este notebook é responsável pela **ingestão do conjunto de dados** e pelas **verificações iniciais de qualidade**, incluindo:

* Estrutura do dataset
* Tipos de variáveis
* Presença de valores ausentes
* Consistência geral dos dados

Nenhuma transformação é realizada nesta etapa. O foco é compreender a base e identificar possíveis limitações ou cuidados necessários para as próximas fases do projeto.

---

### Notebook 2 – Exploração e Análise de Dados (EDA)

Neste notebook é realizada a **análise exploratória dos dados**, com foco na compreensão dos fatores associados ao risco de crédito.

As análises são conduzidas **sempre em função da variável alvo (`target`)**, onde:

* `0` representa clientes adimplentes
* `1` representa clientes inadimplentes

As variáveis categóricas são analisadas em sua forma original, antes de qualquer codificação, priorizando **interpretabilidade**, **análise de padrões** e **storytelling com dados**.

---

### Notebook 3 – Feature Engineering

Este notebook tem como objetivo preparar os dados para a etapa de modelagem preditiva, garantindo:

* Separação clara entre treino e teste
* Ausência de vazamento de dados
* Reprodutibilidade das transformações

São realizadas etapas como:

* Identificação de variáveis numéricas e categóricas
* Definição de pipelines de pré-processamento
* Aplicação de normalização e codificação
* Persistência dos dados processados e do pipeline

Ao final, os conjuntos de dados prontos para modelagem são salvos para uso posterior.

---

### Notebook 4 – Avaliação e Comparação de Modelos

Neste notebook são treinados e avaliados modelos de **Machine Learning** aplicados ao problema de risco de crédito, considerando o contexto de **base desbalanceada**.

São utilizados:

* Um modelo baseline de **Regressão Logística**, priorizando interpretabilidade
* Um modelo de **Random Forest**, explorando relações não lineares

A avaliação considera métricas adequadas ao problema, como:

* Matriz de confusão
* Relatório de classificação
* ROC AUC

Ao final, os modelos são comparados e discutidos sob a ótica de **performance, interpretabilidade e impacto no negócio**.

---

## Tecnologias Utilizadas

* Python
* pandas, numpy
* matplotlib, seaborn
* scikit-learn
* joblib

---

## Considerações Finais

Este projeto foi desenvolvido com foco em **portfólio profissional**, priorizando boas práticas de Ciência de Dados, clareza na comunicação e organização do código.

A estrutura modular dos notebooks permite fácil manutenção, reuso do pipeline e adaptação para cenários reais de risco de crédito em instituições financeiras.

---

## Autor

Aline Brito Lima

Engenheira Eletricista | Cientista de Dados Júnior

Projeto desenvolvido para fins de estudo e portfólio profissional em Ciência de Dados aplicada ao risco de crédito.
