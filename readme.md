![Logo da Ada Tech Crusos](./assets/LogoAdaCabecalho.png)

<hr>

<p></p>
<p align="center">
   <img src="https://img.shields.io/static/v1?label=STATUS&message=%20EM CONSTRUÇÃO&color=RED&style=for-the-badge" #vitrinedev/>
</p>

## <center>PROJETO MACHINE LEARNING I | SANTANDER CODERS 2024 | ADA TECH </center>

# Tópicos 

- [Regras de Colaboração](#regras-de-colaboracao)

- [Descrição do projeto](#descrição-do-projeto)

- [DataSet](#dataset)

- [Funcionalidades](#funcionalidades)

- [Estrutura do Projeto](#estrutura)

- [Ferramentas utilizadas](#ferramentas-utilizadas)

- [Acesso ao projeto](#acesso-ao-projeto)

- [Colaboradores](#colaboradores)

## Regras de Colaboração

Após confirmação do convite no GitHub, recomenda-se:

1. Crie um repositorio local;
2. Clone o projeto: 
```bash
git clone "https://github.com/Polga-Fe/05_MachLearn--coders24/"
```
```bash
git pull
```
3. Crie uma branch com seu nome:
```bash
git checkout -b 'seu_nome' 
```
4. Agora você irá trabalhar dentro da sua branch (verifique no VS Code se está na sua branch)
5. Para subir sua contribuição para a "main", siga os passos:
```bash
git add .
git commit -m "sua contribuição"
git push origin "seu_nome"
```
6. Atualize a "main": 
```bash
git checkout main
git merge "seu_nome"
```
7. Após "mergear", informe ao grupo que você atualizou a "main";
8. Então, os demais colabs devem atualizar a sua "main":
```bash
git pull origin main
```

## Descrição do projeto 

### Santander Coders 2024 - Turma 1174

### Projeto Machine Learning I

Neste projeto, cada grupo irá escolher um dos cinco conjuntos de dados abaixo e desenvolver um modelo de aprendizado supervisionado para resolver o problema proposto. O foco estará em todo o ciclo de desenvolvimento de um projeto de Machine Learning, desde a compreensão dos dados até a avaliação final do modelo. Cada etapa será cuidadosamente planejada para garantir que o modelo seja bem-sucedido na tarefa de predição.

## Dataset

`Dataset Público:` Default of Credit Card Clients Dataset. Default Payments of Credit Card Clients in Taiwan from 2005. From Kaggle [acessar o dataset do projeto](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset).

### UCI_Credit_Card_Kaggle - Sobre o conjunto de dados

Este conjunto de dados contém informações sobre pagamentos inadimplentes, fatores demográficos, dados de crédito, histórico de pagamentos e extratos de contas de clientes de cartão de crédito em Taiwan, abrangendo o período de abril de 2005 a setembro de 2005.

### Conteúdo do Conjunto de Dados

| Variável                       | Descrição                                                                                                 |
|--------------------------------|-----------------------------------------------------------------------------------------------------------|
| `ID`                           | ID de cada cliente                                                                                        |
| `LIMIT_BAL`                    | Valor do crédito fornecido em dólares NT (inclui crédito individual e familiar/suplementar)               |
| `SEXO`                         | Gênero (1=masculino, 2=feminino)                                                                          |
| `EDUCAÇÃO`                     | Nível educacional (1=pós-graduação, 2=universidade, 3=ensino médio, 4=outros, 5=desconhecido, 6=desconhecido) |
| `CASAMENTO`                    | Estado civil (1=casado, 2=solteiro, 3=outros)                                                            |
| `IDADE`                        | Idade em anos                                                                                             |
| `PAY_0`                        | Situação do pagamento em setembro de 2005 (-1=pagar em dia, 1=atraso no pagamento por um mês, ..., 9=atraso de nove meses ou mais) |
| `PAY_2`                        | Situação do pagamento em agosto de 2005 (mesma escala de PAY_0)                                          |
| `PAY_3`                        | Situação do pagamento em julho de 2005 (mesma escala de PAY_0)                                           |
| `PAY_4`                        | Situação do pagamento em junho de 2005 (mesma escala de PAY_0)                                           |
| `PAY_5`                        | Situação do pagamento em maio de 2005 (mesma escala de PAY_0)                                            |
| `PAY_6`                        | Situação do pagamento em abril de 2005 (mesma escala de PAY_0)                                           |
| `BILL_AMT1`                    | Valor da fatura em setembro de 2005 (dólar NT)                                                           |
| `BILL_AMT2`                    | Valor da fatura em agosto de 2005 (dólar NT)                                                             |
| `BILL_AMT3`                    | Valor da fatura em julho de 2005 (dólar NT)                                                              |
| `BILL_AMT4`                    | Valor da fatura em junho de 2005 (dólar NT)                                                              |
| `BILL_AMT5`                    | Valor da fatura em maio de 2005 (dólar NT)                                                               |
| `BILL_AMT6`                    | Valor da fatura em abril de 2005 (dólar NT)                                                              |
| `PAY_AMT1`                     | Valor do pagamento anterior em setembro de 2005 (dólar NT)                                              |
| `PAY_AMT2`                     | Valor do pagamento anterior em agosto de 2005 (dólar NT)                                                |
| `PAY_AMT3`                     | Valor do pagamento anterior em julho de 2005 (dólar NT)                                                 |
| `PAY_AMT4`                     | Valor do pagamento anterior em junho de 2005 (dólar NT)                                                 |
| `PAY_AMT5`                     | Valor do pagamento anterior em maio de 2005 (dólar NT)                                                  |
| `PAY_AMT6`                     | Valor do pagamento anterior em abril de 2005 (dólar NT)                                                 |
| `default.payment.next.month`   | Inadimplência de Pagamento (1=sim, 0=não)


## Funcionalidades

`Funcionalidade 1:` Modelagem de Machine Learning.


## Estrutura do Projeto

`1. Entendimento do Problema e Definição de Objetivos` 
• Tarefa: Analisar o problema proposto pelo conjunto de dados escolhido. Entender a natureza do problema (classificação binária, multiclasse ou regressão) e definir claramente os objetivos do projeto.
• Exemplo: No caso do Telco Customer Churn, o objetivo será prever se um usuario faz parte do churn ou não.

`2. Coleta e Preparação de Dados`
• Tarefa: Realizar o carregamento do dataset e fazer uma análise exploratória inicial. Isso inclui uma análise detalhada das variáveis, tipos de dados, presença de valores nulos ou inconsistências. 
•    Subtarefas:
•    Remover ou preencher valores ausentes.
•    Normalizar e padronizar as variáveis (se necessário).
•    Codificar variáveis categóricas (se aplicável).

`3. Análise Exploratória de Dados (EDA)`
• Tarefa: Realizar uma análise exploratória de dados aprofundada para entender as correlações entre as variáveis, distribuições e possíveis padrões. • Subtarefas: • Criar gráficos (distribuição, histogramas, box plots, etc.). • Analisar correlações entre as variáveis. • Identificar variáveis que podem ser eliminadas ou combinadas.

`4. Divisão dos Dados em Conjuntos de Treinamento e Teste`
• Tarefa: Dividir o dataset em treinamento e teste (usualmente 80%/20%) para garantir a capacidade do modelo de generalizar bem a novos dados.

`5. Escolha e Implementação de Algoritmos`
• Tarefa: Escolher um ou mais algoritmos de aprendizado supervisionado para treinar o modelo. Testar diferentes algoritmos e ajustar seus hiperparâmetros para melhorar a performance.
• Algoritmos sugeridos: Logistic Regression, Decision Trees, Random Forest, KNN Classifier/Regression etc.

`6. Avaliação do Modelo`
• Tarefa: Avaliar o desempenho do modelo usando métricas apropriadas para o tipo de problema.
• Classificação: • Métricas: Acurácia, Precisão, Revocação, F1-Score, AUC-ROC. • Regressão: • Métricas: RMSE, MAE, R².

`7. Ajuste de Hiperparâmetros e Tuning do Modelo`
• Tarefa: Utilizar técnicas como Grid Search ou Random Search para ajustar hiperparâmetros e melhorar o desempenho do modelo.

`8. Validação Cruzada e Teste Final`
• Tarefa: Aplicar validação cruzada para verificar a robustez do modelo e garantir que ele não esteja superajustado (overfitting). Em seguida, realizar o teste final no conjunto de teste.

`9. Interpretação dos Resultados e Conclusão`
• Tarefa: Interpretar os resultados do modelo, destacando insights importantes, limitações e sugestões para melhorias futuras.

`10. Relatório Final`
• Tarefa: Cada grupo deve compilar um relatório que inclua:
• Descrição do problema.
• Explicação da preparação e exploração de dados.
• Justificativa da escolha dos algoritmos.
• Análise dos resultados e gráficos gerados.
• Conclusão com possíveis melhorias futuras.
• Código comentado.

Nota: Este relatório pode ser feito no próprio notebook da modelagem

`Avaliação do Projeto`

A avaliação do projeto será feita com base nos seguintes critérios:
• Qualidade e profundidade da análise exploratória.
• Eficiência e desempenho do modelo criado.
• Clareza do relatório final e apresentação dos resultados.
• Qualidade do código desenvolvido.

## Ferramentas utilizadas

[![My Skills](https://skillicons.dev/icons?i=git,github,python)](https://skillicons.dev)

###

## Acesso ao projeto

Você pode [acessar o código fonte do projeto](https://github.com/Polga-Fe/05_MachLearn--coders24/).

## Colaboradores

| [<img src="https://avatars.githubusercontent.com/u/7073699?v=4" width=115> <br><sub>Instrutor ADA Joelson Antônio dos Santos</sub>](https://github.com/joelsonSantos) |  [<img src="https://avatars.githubusercontent.com/u/60614096?v=4" width=115><br><sub>Diogo Carvalho</sub>](https://github.com/Dogix11) | [<img src="https://avatars.githubusercontent.com/u/167734497?v=4" width=115> <br><sub>Fernanda N</sub>](https://github.com/Polga-Fe) | [<img src="https://avatars.githubusercontent.com/u/161227020?v=4" width=115><br><sub>Giovana Gabi</sub>](https://github.com/rhapozita) | [<img src="https://avatars.githubusercontent.com/u/130763076?v=4" width=115><br><sub>Luiza Simões</sub>](https://github.com/ ) |  [<img src="https://avatars.githubusercontent.com/u/170963236?s=96&v=4" width=115><br><sub>João Oliveira</sub>](https://github.com/jjofilho) |
| :---: | :---: | :---: | :---: | :---: | :---: |
