# Extract, Transform and Load (ETL)

## Índice
- [Nomes](#nomes)
- [Objetivo](#objetivo)
- [Dataframe de Dados](#dataframe-de-dados)
- [Dataframe de Resultados](#dataframe-de-resultados)
- [Artigo](#artigo)
- [Como Usar](#como-usar)
- [Dependências](#dependencias)

## Nomes
* Alice Vitória Boschetti
* Eduardo Marques dos Santos
* Felipe Cordeiro Carvalho
* Gabriel Frigo Sena Silva
* Joyce Nunes Alves
* Kimberly Oliveira Germano Ribeiro

## Objetivo
* Este projeto tem como objetivo a medição de 100 bolinhas de gude com paquímetro e seu tratamento de dados a fim de obter análise de gráficos para a distribuição de medidas e cálculo de incertezas.
  
![Medição](./pictures/medicao.png)

## Dataframe de Dados  

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

![Dataframe de Dados](./pictures/medicao.png)

## Dataframe de Resultados

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

![Dataframe de Resultados](./pictures/medicao.png)

## Drivers
* Http Requester: Utilizar a url do website para fazer uma requisição HTTP utilizando a lib Requests e obtém uma resposta (status code e conteúdo do HTML);
* Html Collector: Foi utilizado o BeautifulSoup para realizar HTML parser e acessar o conteúdo de uma classe específica HTML ("BodyText") e obter os valores de uma tag <a>. Aqui é retornado o nome do artista e o seu link.

## Extração
* Utiliza dos dados provenientes do Http Resquester e HTML Collector para extração; 
* Retorno: Conteúdo (raw_information_content) e Data da Extração (extraction_date)

## Transformação
* Com o retorno raw_information_content, faz a separação das variáveis necessárias interagindo com as strings;

## Carregamento
* Em "Infra/database_connector" é feito o script para conexão com o banco de dados local utilizando DBeaver e MySQL;
* Em "Infra/database_repository" é feito o script para query de criação do database;
* A etapa de carregamento une os itens anteriores para criação do database e inserção de dados com a query criada.

* Resultado:
![Load](./load.PNG)

## Como Usar



## Dependências
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
