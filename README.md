# CasePetLove

# leitura e tratamento de dados

## Imports Necessários
Começamos o projeto importando as bibliotecas necessárias para ler e explorar os dados disponibilizados.

![Imports](./prints/1.JPG)

## leitura do dataset
logo em seguida usamos o pandas para fazer a leitura do arquivo juntamente com a biblioteca requests para não precisar baixar o arquivo e fazer a leitura de forma local

![Imports](./prints/2.JPG)

## tratamento do dataset
Alguns tratamentos que julguei necessarios como conversão de textos em datas e criação de novas features que não continham no data set original tais como idade e o total de dias que um cliente ficou sem realizar compra antes de cancelar a assinatura.

![Imports](./prints/3.JPG)

## encoder de variáveis categóricas
Alguns dados importantes vieram como labels, utilizei o label enconder da biblioteca scikit-learn para realizar o encoder dessas variaveis e criei uma copia do dataset

![Imports](./prints/4.JPG)


# análise exploratória

## Primeira análise 
Verificando o balancemento do dataset em relação ao status

![Imports](./prints/5.JPG)

## Segunda análise 
Em busca de alguma discrepância nos dados de "Marketing Source"

![Imports](./prints/6.JPG)

## terceira análise 
Plot de gráficos das 8 variáveis de medida por status, na tentativa de encontrar algum dado sobressaltante nessas medidas

![Imports](./prints/6.1.JPG)

Após o plot dos gráficos ficou claro que o total de dias sem comprar antes do cancelamento é um dos pontos importantes

## Quarta análise
Utilizando seaborn para plotar um mapa de calor com as correlações das features, que exibiu as medidas "Recency" e "days_without_buying_before_canceling" com a maior correlação com o "Status"

![Imports](./prints/7.JPG)

## Quinta análise
Criação de um modelo utilizando RandomForestClassifier para plotar um gráfico com as features mais importantes do dataset

![Imports](./prints/8.JPG)

