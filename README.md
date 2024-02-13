<h1>Azure - Machine Learning</h1>
<p align="center">
Exercício de aprendizado de Máquinas utilizando o Azure para treinar e avaliar o cenário de aluguel de bicileta.
</p>

## 📎 Introdução

- Para começarmos a utilizar a Plataforma ML é necessário criar um recurso de Machine Learning na Azure.
- Após a criação do recurso será necessário configurar um ambiente de trabalho, todas os códigos e passo a passo do projeto estão na documentação da <a href="https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/01-machine-learning.html">Microsoft</a>
- Neste exercício estamos trabalhando com um modelo de aprendizado baseado em dados históricos, sobre aluguel de bicicleta, todas as informações para sustentar nosso modelo está sendo oferecida pelo <a href="https://aka.ms/bike-rentals">Bike Rentals</a>, durante a configuração de aprendizado será necessário realizar algumas configurações também oferecidas na documentação.
- Após configurado e treinado o modelo é possível avaliar os resultados do treinamento, na qual contamos com dois gráficos sendo eles o predicted_true, que nos oferece uma previsão e um valor ideal e o residuals que consistem em um Histograma.
- Para implantar o modelo é necessário informar dados no formatos JSON que irão nos trazer uma probabilidade de retorno. Segue abaixo os dados de entrada e uma estímativa de saída

## Entrada

```
{
  "Inputs": {
    "data": [
      {
        "day": 0,
        "mnth": 0,
        "year": 0,
        "season": 0,
        "holiday": 0,
        "weekday": 0,
        "workingday": 0,
        "weathersit": 0,
        "temp": 0.0,
        "atemp": 0.0,
        "hum": 0.0,
        "windspeed": 0.0
      }
    ]
  },
  "GlobalParameters": 0.0
}
```

## Saída

```
 {
   "Results": [
     0: float 440.65842387505177
   ]
 }
```