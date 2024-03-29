# Física Aplicada: Experimento Bolinhas de Gude

## Índice
- [Nomes](#nomes)
- [Como Usar](#como-usar)
- [Objetivo](#objetivo)
- [Dataframe](#dataframe)
- [Resultados](#resultados)
- [Fórmulas](#fórmulas)
- [Bibliotecas](#bibliotecas)

## Nomes
* Alice Vitória Boschetti
* Eduardo Marques dos Santos
* Felipe Cordeiro Carvalho
* Gabriel Frigo Sena Silva
* Joyce Nunes Alves
* Kimberly Oliveira Germano Ribeiro

## Como Usar
Abaixo está descrito a função de cada arquivo dentro da estrutura do projeto. Baixe a pasta completa e execute no Google Colab ou Jupyter Notebook:

* `extract_excel_save_csv`: Arquivo que extrae de uma fonte Excel a tabela com dados brutos e realiza o tratamento bem como a aplicação das equações;
* `analytics`: Arquivo que reúne o dataframe e os dataframe de resultados para analisar graficamente a distribuição das bolinhas e suas incertezas;
* `data`: Contém os dados salvos em csv;


## Objetivo
* Este projeto tem como objetivo a medição de 100 bolinhas de gude com paquímetro e seu tratamento de dados a fim de obter análise de gráficos para a distribuição de medidas e cálculo de incertezas;
* Link para artigo:  https://drive.google.com/file/d/1JmDJJ7q-TETmhPR0_8GV0-Xl8vbq94zw/view?usp=sharing
  
![Medição](./pictures/medicao.PNG)


## Dataframe 

| Nome da Variável            | Descrição                                                       |
|-----------------------------|-----------------------------------------------------------------|
| D1                   | Diâmetro respectivo ao lado 1 da bolinha. |
| D2                | Diâmetro respectivo ao lado 2 da bolinha. |
| diferenca_D1_D2                        | Diferença entre medidas (d = D2-D1). |
| desvio_absoluto_D1                | Cálculo desvio absoluto para diâmetro 1. |
| desvio_absoluto_D2                         | Cálculo desvio absoluto para diâmetro 2. |
| volume_V1                         | Volume da bolinha utilizando o raio do diâmetro 1. |
| volume_V2                         | Volume da bolinha utilizando o raio do diâmetro 2. |
| diferença_V1_V2                         |  Diferença entre volumes (V = V2-V1). |
| desvio_absoluto_V1                         | Cálculo desvio absoluto para diâmetro 1. |
| desvio_absoluto_V2                         | Cálculo desvio absoluto para diâmetro 2. |

Abaixo está uma foto do dataframe e saus variáveis usadas para o cálculo dos resultados finais:

![Dataframe](./pictures/dataframe.png)

## Resultados

| Nome da Variável            | Descrição                                                       |
|-----------------------------|-----------------------------------------------------------------|
| Incerteza Absoluta D1	                   | Valor médio de D1 e desvio absoluto de D1 |
| Incerteza Absoluta D2	                | Valor médio de D2 e desvio absoluto de D2. |
| Incerteza Média D1	                        | Valor médio de D1 e desvio médio de D1. |
| Incerteza Média D2	                | Valor médio de D2 e desvio médio de D2. |
| Incerteza Absoluta V1                         |  Valor médio de V1 e desvio absoluto de V1. |
| Incerteza Absoluta V2                         | Valor médio de V2 e desvio absoluto de V2. |
| Incerteza Média V1	                         | Valor médio de D1 e desvio médio de D1. |
| Incerteza Média V2	                         |   Valor médio de D2 e desvio médio de D2. |

Abaixo está uma foto do dataframe com os resultados finais:

![Medição](./pictures/dataframe_resultados.PNG)

## Fórmulas
* `Desvio Absoluto:`

![Desvio Absoluto](./pictures/absoluto_2.PNG)

* `Desvio Médio:`

![Desvio Médio](./pictures/desv_med_1.PNG)

## Bibliotecas
Copie e instale as dependências abaixo:

```bash
pip install pandas
```
```bash
pip install numpy
```
```bash
pip install plotly-express
```
