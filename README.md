# Previsão utilizando Poisson

Realização de desafio de previsão de ocorrência de um evento utilizando python, pandas e probabilidade.
A técnica escolhida foi a de poisson. 

### $$ \text{Distribuição de Poisson:} \quad P(X = k) = \frac{{\lambda^{k}x^\lambda}}{k!}$$

A distribuição de Poisson é uma distribuição de probabilidade discreta que descreve a probabilidade de um número específico de eventos ocorrer em um intervalo fixo de tempo, espaço ou volume, desde que os eventos ocorram de forma independente e com uma taxa média constante.

def distribuicao_poisson(l: float, k: int) -> float:
    return ((l**k) * np.exp(-l)) / math.factorial(k)

