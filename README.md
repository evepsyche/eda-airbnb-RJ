# Análise Exploratória dos dados do Airbnb do Rio de Janeiro.
<img src="https://images.unsplash.com/photo-1626568940331-b9efa277b000?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80" alt="RJ">

[Artigo no Medium](https://medium.com/@lainetnr/análise-exploratória-de-dados-eda-com-python-airbnb-no-rio-de-janeiro-68ad7ef2e93a) sobre a análise.
## Sobre os dados
Os dados foram coletados através do portal [Inside Airbnb]( https://insideairbnb.com/get-the-data ) e o arquivo utilizado foi o de nome 'listings.csv' que refere-se a informações resumidas e métricas para listagens no Rio do Janeiro, como é descrito no próprio portal. Também foi usado o arquivo 'neighbourhoods.geojson', com geolocalização para criação de um mapa interativo.

## Entendendo o objetivo da análise
O objetivo da análise é retirar insights a fim de resolver problemas de negócio usando os dados para responder perguntas.

As perguntas em questão são:

* Quais os principais tipos de imóveis locados na cidade do Rio de Janeiro?
* Quais as medianas dos preços dos aluguéis para cada tipo de imóvel?
* Quais as médias de preços dos bairros mais caros e mais baratos da cidade do Rio de Janeiro?
* Qual a disponibilidade médias dos imóveis na cidade do Rio de Janeiro?

## Métodos
  * Limpeza dos dados
  * Análise Exploratória de Dados
  * Visualização de Dados

## Tecnologias
  * Python
  * Google Colab
  * Matplotlib
  * Seaborn 
  * Pandas
  * Numpy

## Insights obtidos
### Q1 -  Quais os principais tipos de imóveis locados na cidade do Rio de Janeiro?
![q1](https://github.com/silvaelaine/eda-airbnb-RJ/assets/103846225/462967d3-f7cb-4608-ba71-d142ebb2ea2c)

* 87% dos imóveis alugados são do tipo casa/apartamento inteiro.
* 12,2% dos imóveis alugados são do tipo quarto privado.
* Quarto de hotel(quarto inteiro ou compartilhado) ficou apenas com 0,051%


### Q2 - Quais as medianas dos preços dos aluguéis para cada tipo de imóvel?
![q2](https://github.com/silvaelaine/eda-airbnb-RJ/assets/103846225/abdc617a-f3eb-44d3-a54e-6b4a89a77af8)

A mediana é o valor central do nosso conjunto de dados. Ela coloca os valores ordenados em ordem crescente e divide os dados em 50%. Podemos ver que os quartos de hotel tem a mediana de preço maior do que os imóveis que alugam a casa/apartamento inteiros!

### Q3 - Quais as médias de preços dos bairros mais caros e mais baratos da cidade do Rio de Janeiro?
![q3](https://github.com/silvaelaine/eda-airbnb-RJ/assets/103846225/3e2baf4c-565d-4d41-bcf9-20f01d64b321)

![q32](https://github.com/silvaelaine/eda-airbnb-RJ/assets/103846225/ae5bd359-0bad-4afa-8b9b-ddc335bb70a8)

### Q4 - Qual a disponibilidade médias dos imóveis na cidade do Rio de Janeiro?
![q4](https://github.com/silvaelaine/eda-airbnb-RJ/assets/103846225/4f34c4c2-7f8e-4171-a3c8-b292fc1b6c94)

O gráfico de distribuição acumulada é muito informativo. Com ele podemos ver que 60% das alocações tem menos de 200 dias disponíveis para alocação. Podemos ver também que apenas 20% tem menos de 100 dias disponíveis para alocação. A média de disponibilidade é de 158,54 dias, com desvio padrão de 106,21 dias, mediana de 139 dias, com disponibilidade mínima de 0 dias e disponibilidade máxima de 365 dias.

### Mapa interativo do preço médio dos aluguéis por bairro
![mapa](https://github.com/silvaelaine/eda-airbnb-RJ/assets/103846225/8a1b6ca9-36e0-43cc-a97e-6825dd4533d1)
Para melhor visualização do mapa é aconselhável abrir o [notebook](https://colab.research.google.com/github/lainetnr/ds-project-airbnb-01/blob/main/EDA_Airbnb_RJ_P01.ipynb#scrollTo=zXqMhFiQP5Qg). Assim, será possível ver a média de preço médio por bairro.

