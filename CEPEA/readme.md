### Centro de Estudos Avançados em Economia Aplicada - CEPEA

## Notícias em Inglês extraido do site do CEPEA

O dataset é sobre notícias das principais commodity do Brasil na língua Inglesa e seus respectivos valores diários.

## Links
* [CEPEA Notícias](https://www.cepea.esalq.usp.br/en/category/brazilian-agribusiness-news.aspx)
* [Valores Milho](https://www.cepea.esalq.usp.br/br/indicador/milho.aspx)
* [Valores Soja](https://www.cepea.esalq.usp.br/br/indicador/soja.aspx)
* [Valores Etanol](https://www.cepea.esalq.usp.br/br/indicador/etanol.aspx)
* [Valores Café](https://www.cepea.esalq.usp.br/br/indicador/cafe.aspx)
* [Valores Algodão](https://www.cepea.esalq.usp.br/br/indicador/algodao.aspx)
* [Valores Trigo](https://www.cepea.esalq.usp.br/br/indicador/trigo.aspx)
* [Valores Açucar](https://www.cepea.esalq.usp.br/br/indicador/acucar.aspx)
* [Valores Boi Gordo](https://www.cepea.esalq.usp.br/br/indicador/boi-gordo.aspx)

## Algoritmo para realizar o Scraping das informações dos links 

Colab : https://colab.research.google.com/drive/1uIlusgfpTcFqqz8jwJvK322iPGCqwiCB?usp=sharing

## Descrição das Colunas 
* Date: data da publicação da notícia;
* Text_Headline: manchete da notícia;
* Text_Body: corpo do texto da notícia;
* Commodity: nome da commodity que a notícia está relacionada;
* Language: língua que a notícia está escrita;
* Real: valor da commodity do dia na moeda Real; e,
* Dolar: valor da commodity do dia na moeda Dolar.

## Carregar e ler arquivo

...
```
import pandas as pd

dataset = pd.read_excel('https://github.com/ivanfilhoreis/agricultural_commodity_data/blob/main/CEPEA/commodity.xlsx?raw=true')

dataset.head()

