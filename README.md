# Previsão de Rotatividade de Clientes (Churn)

<sub>TAGS: Pandas; Numpy; Scikit-Learn; Matplotlib; Seaborn; XGBoost; Feature Engineering; Feature Scaling; Cross Validation; GridSearchCV; Pipeline

<p align="center">
  <img src="capa_p4.png" >
</p>

## Objetivos

Este projeto buscou conhecer melhor os motivos para as taxas de rotatividade em uma empresa de telecomunicações, utilizando-se de dados históricos de seus clientes.

- Aquisição dos dados;
- Análise Exploratória dos dados;
- Pré-processamento dos dados;
- Construção de modelos de Machine Learning (ML);
- Otimização de hiperparâmetros;

O objetivo final é apresentar modelos viáveis para predição de rotatividade, diminuindo as taxas de saídas dos clientes de acordo com as circunstâncias particulares impostas pelo problema de negócio em questão.

### Relevância

O Churn é fonte de muita preocupação para empresas dos mais diversos nichos, desde o entretenimento até prestações de serviços, pois se relaciona diretamente com a perda de lucro devido à saída de clientes.

Por este motivo, é relevante utilizar dos dados para ter uma consciência situacional maior dos motivos por trás da saída de um cliente. Com a construção de modelos de Machine Learning através de dados históricos, a empresa é capaz de identificar os perfis dos clientes mais propensos à rotatividade e, a partir disso, tomar iniciativas voltadas para mantê-los e fidelizá-los.

## Conclusões

A partir de testes com diversos algoritmos de classificação, escolheu-se aprimorar três modelos segundo sua versatilidade na otimização de hiperparâmetros. Foram escolhidos os modelos de SGD (Classificador Linear de Descida de Gradiente Estocástico), LightGBM (Classificador de Impulsionamento de Gradiente Leve) e o XGBoost (Classificador por Impulsionamento de Gradiente Extremo).

Os três modelos preveem a rotatividade de maneira eficiente, porém com diferenças que podem ser proveitosas segundo as circunstâncias específicas da empresa e do problema de negócios. 

- O **SGD Classifier** possui uma performance equilibrada, com uma boa previsão de rotatividade, e uma taxa razoável de Falsos Negativos. **(Recall:  0.835 ± 0.019)**
- O **LightGBM Classifier** é o menos capaz de prever a rotatividade, com uma taxa de Falsos Negativos de aproximadamente 20%. Porém, ele é o melhor na distinção de classes e sua taxa de Falsos Positivos é a mais baixa. **(Recall:  0.793 ± 0.019)**
- Por último, o **XGBoost Classifier** é o melhor modelo para previsão de rotatividade, com uma taxa de quase 90%. Contudo, é o que pior performa na taxa de Falsos Positivos. **(Recall:  0.883 ± 0.022)**

<sub>[Retornar ao Portfólio](https://github.com/gabrielrflopes/Data-Science-Portfolio/tree/main)
