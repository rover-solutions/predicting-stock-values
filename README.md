# Previsão de Preços de Ações com Modelos de Regressão e Séries Temporais

A previsão de preços de ações na bolsa de valores é um problema complexo que chama o olhar de investidores e pesquisadores há décadas. A utilização de modelos de regressão e séries temporais pode ajudar a prever a direção futura dos preços das ações, mas é importante avaliar a qualidade desses modelos para garantir que suas previsões sejam confiáveis e úteis.

Existem várias métricas que podem ser usadas para avaliar modelos de regressão e séries temporais, incluindo o erro médio absoluto (MAE), o erro quadrático médio (MSE) e o coeficiente de determinação (R²). O MAE mede a diferença média entre as previsões do modelo e os valores reais, enquanto o MSE mede a média dos quadrados das diferenças entre as previsões e os valores reais. O R² é uma medida de quão bem as previsões do modelo se ajustam aos dados reais.

Neste exemplo, estamos carregando os dados históricos de preços da AAPL a partir de um arquivo CSV. Em seguida, criamos uma nova coluna com os preços de fechamento deslocados um dia para frente, para usá-los como nossa variável de saída. Depois, separamos os dados em um conjunto de treinamento e um conjunto de teste.

Para o modelo de regressão linear, criamos as variáveis de entrada e saída, treinamos o modelo e fizemos previsões no conjunto de teste. Em seguida, avaliamos as métricas de desempenho do modelo (MAE, MSE e R²).

Para o modelo de séries temporais, criamos as variáveis de entrada e saída, treinamos o modelo ARIMA e fizemos previsões no conjunto de teste.

Nesse exemplo, as métricas obtidas para cada modelo foram:
```
Métricas do Modelo de Regressão Linear:
MAE: 1.9320762133592926
MSE: 31.33040333355253
R²: 0.9811016981730226

Métricas do Modelo de Séries Temporais (ARIMA):
MAE: 71.28566517163931
MSE: 6798.338154870248
R²: -3.122203322270132
```

- MAE (Mean Absolute Error) é a média das diferenças absolutas entre as previsões e os valores reais. Quanto menor o valor do MAE, melhor é o desempenho do modelo. No caso do modelo de regressão linear.

- MSE (Mean Squared Error) é a média dos quadrados das diferenças entre as previsões e os valores reais. O MSE é uma métrica que penaliza mais os erros maiores. Quanto menor o valor do MSE, melhor é o desempenho do modelo. Isso indica que o modelo de regressão linear apresentou um desempenho um pouco melhor que o modelo ARIMA, uma vez que seu MSE foi menor.

- R² (Coefficient of determination) é uma medida que indica o quanto da variação dos valores de saída pode ser explicada pelas variáveis de entrada. Quanto mais próximo de 1 o valor de R², melhor é o desempenho do modelo. No caso do modelo de regressão linear, o R² foi de 0.98, o que indica que as variáveis de entrada explicam uma pequena parte da variação dos valores de saída. Já no modelo ARIMA, o R² foi de -3.122, o que indica um desempenho muito ruim do modelo, pois o valor negativo indica que o modelo não explica a variação dos valores de saída.

