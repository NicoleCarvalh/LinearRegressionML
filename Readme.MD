# Machine Learning - Análise de acidentes fatais de trânsito na Australia entre 1989 e 2021

_Nesse projeto estamos criando um modelo de aprendizado de maquina (machine learning) para analisar os dados, extrais insights e aplicando conceitos como o treino e teste do modelo, aplicação de métricas de classificação, métricas de regressão linear, análise gráfica através da plotagem dos dados e demais conceitos._

## Contexto e preparação

### Dataset
Como base de dados inicial, buscamos dentro da plataforma <a href='https://www.kaggle.com/'>Kaggle</a>, um dataset com mais de 15mil registros. 

Dentre os datasets e estudos presentes na plataforma, escolhemos utilizar o dataset sobre os acidentes fatais de trânsito na Australia, com dados históricos entre as datas de 1989 e 2021. 

Dataset original: <a href='https://www.kaggle.com/datasets/deepcontractor/australian-fatal-car-accident-data-19892021'>Australian Fatal Road Accident 1989-2021</a>

> Obs: o dataset fornecido está em formato .csv

### Preparando o dataset para os estudos
Foram utilizadas bibliotecas que auxiliam no manuseio de dados, como:

- pandas
- seaborn
- matplotlib
- numpy
- sklearn

Dentre outras presentes no arquivo 'requirements.txt' do projeto.


## Conceitos importantes

### X e Y: Características e Rótulos
- X: Representa as características (features) dos seus dados. No contexto de acidentes de trânsito, isso pode incluir variáveis como hora do dia, condições climáticas, tipo de veículo, etc.

- Y: Representa a variável alvo (target) que você deseja prever. Isso pode ser uma classificação (e.g., acidente ou não acidente) ou um valor numérico (e.g., número de feridos).
  
- O *label encoding* serve para transformar variáveis categóricas em números, facilitando o uso em algoritmos que requerem entradas numéricas. Ele não deve ser usado quando as categorias não têm uma ordem natural ou contínua (como dias da semana ou cores).
  - Para variáveis categóricas sem ordem, como os dias da semana, é melhor usar *one-hot encoding* ou algoritmos que lidam diretamente com categorias (como árvores de decisão, Random Forest, etc.).

### Treino e teste

Antes de realizarmos o treino e teste com um modelo, precisamos entender qual o nosso alvo (qual valor queremos prever/classificar).

Após identifica-lo, nós separamos ele em uma variavel chamada 'Y' e o resto do dataset (sem a coluna Y) nós armazenamos em uma variavel 'X'



## Possíveis previsões e classificações

