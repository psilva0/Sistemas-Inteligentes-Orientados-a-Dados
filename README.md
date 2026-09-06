# Sistemas-Inteligentes-Orientados-a-Dados
Repositório para projeto da matéria: Sistemas Inteligentes Orientados a Dados - PGCOMP - UFBA

Electoral Demand Prediction - ML for Social Impact

1. Problema

Como prever quais zonas eleitorais apresentarão maior demanda de eleitores em uma próxima eleição para apoiar o planejamento e a distribuição de recursos eleitorais?

2. Objetivo

Desenvolver um modelo de Machine Learning capaz de utilizar dados históricos de eleições para identificar zonas eleitorais que poderão apresentar maior demanda de eleitores em uma eleição futura.

A proposta é utilizar padrões históricos de comparecimento e características eleitorais como apoio ao planejamento da estrutura e da distribuição de recursos eleitorais.

3. Dados

O projeto utiliza dados históricos de eleições brasileiras disponibilizados pelo Tribunal Superior Eleitoral (TSE), contemplando registros entre 1994 e 2024.

Entre as principais informações disponíveis estão:

número de eleitores aptos;

comparecimento;

abstenções;

votos válidos;

votos brancos e nulos;

proporção de comparecimento;

zona eleitoral;

município;

unidade federativa;

cargo;

tipo de eleição;

data da eleição.

A análise inicial da fonte de dados identificou registros de eleições não ordinárias, registros associados à identificação ZZ e algumas inconsistências pontuais entre variáveis eleitorais. Esses casos foram investigados e tratados de acordo com sua relação com o problema.

4. Abordagem

O projeto utiliza uma estratégia de modelagem temporal. Informações de eleições anteriores serão utilizadas para construir variáveis defasadas (lags), permitindo que o modelo seja treinado com dados históricos e avaliado em períodos posteriores.

A abordagem contempla:

análise exploratória dos dados;

avaliação da qualidade dos dados;

engenharia de atributos;

construção de variáveis temporais;

prevenção de data leakage;

validação temporal;

comparação de modelos de Machine Learning;

avaliação das previsões;

interpretabilidade dos modelos.

5. Limitações

Os dados eleitorais apresentam particularidades relacionadas a diferentes tipos de eleição, cargos e períodos históricos. Por isso, os registros foram analisados antes da modelagem e as decisões de tratamento foram baseadas na consistência dos dados e na relação com o problema.

As previsões do modelo representam padrões estatísticos identificados nos dados históricos. Portanto, o sistema deve ser entendido como uma ferramenta de apoio ao planejamento e à tomada de decisão, e não como substituto da análise das autoridades responsáveis pela organização eleitoral.

6. Atividade 01 - Caracterização e avaliação inicial dos dados

A primeira etapa do projeto consiste na caracterização técnica e avaliação inicial da fonte de dados, verificando sua disponibilidade, qualidade e limitações.

A documentação da atividade está disponível em:

docs/atividade-01-dados.md

A análise exploratória reproduzível está disponível em:

notebooks/01_exploracao_dados.ipynb
