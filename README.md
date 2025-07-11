# Análise de Algoritmos de Ordenação em C

Este projeto implementa e analisa o desempenho de três algoritmos de ordenação (Bubble Sort, Selection Sort e Quick Sort) aplicados a uma estrutura de dados `Pessoa`, ordenando-a em ordem alfabética pelo nome.

## Algoritmos Escolhidos

Foram implementados os seguintes algoritmos:

### 1. Bubble Sort
O Bubble Sort é um algoritmo simples que percorre repetidamente a lista, compara elementos adjacentes e os troca se estiverem na ordem errada. As passagens pela lista são repetidas até que a lista esteja ordenada. É conhecido por sua simplicidade, mas também por sua ineficiência em grandes conjuntos de dados.

### 2. Selection Sort
O Selection Sort divide a lista em duas partes: uma sublista ordenada e uma sublista com os itens restantes. A cada iteração, ele encontra o menor elemento na sublista não ordenada e o coloca no final da sublista ordenada. Ele se destaca por realizar um número mínimo de trocas.

### 3. Quick Sort
O Quick Sort é um algoritmo de "dividir para conquistar" muito eficiente. Ele seleciona um elemento como "pivô" e particiona os outros elementos em dois sub-arrays, de acordo com o fato de serem menores ou maiores que o pivô. Os sub-arrays são então ordenados recursivamente.

## Complexidade dos Algoritmos

A complexidade de tempo descreve como o tempo de execução de um algoritmo cresce com o tamanho da entrada ($n$).

| Algoritmo       | Tempo (Melhor Caso) | Tempo (Médio)     | Tempo (Pior Caso) | Espaço (Pior Caso) |
|-----------------|---------------------|-------------------|-------------------|--------------------|
| **Bubble Sort** | $O(n)$              | $O(n^2)$          | $O(n^2)$          | $O(1)$             |
| **Selection Sort**| $O(n^2)$            | $O(n^2)$          | $O(n^2)$          | $O(1)$             |
| **Quick Sort** | $O(n \log n)$       | $O(n \log n)$     | $O(n^2)$          | $O(\log n)$        |

## Resultados Obtidos

Os resultados abaixo foram calculados a partir da ordenação de um array de 2.000 elementos, com o tempo médio de 5 execuções consecutivas.

| Algoritmo       | Número de Comparações | Número de Trocas | Tempo Médio (ms) |
|-----------------|-----------------------|------------------|------------------|
| **Bubble Sort** | *713415* | *359944* | *28.6000 ms* |
| **Selection Sort**| *713415* | *1185* | *9.2000 ms* |
| **Quick Sort** | *74395* | *35645* | *3.0000 ms* |
