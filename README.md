# Análise do Consumo de Energia Elétrica em Alagoas (2010–2025)

Análise em Python de dados públicos sobre o consumo de energia elétrica por município e por classe de consumo em Alagoas, mostrando a evolução ao longo dos anos, os municípios que mais consomem e o consumo por consumidor.

## Objetivo

Transformar uma base pública extensa em informações fáceis de entender, respondendo:

- Como o consumo total evoluiu ao longo dos anos?
- Quais municípios mais consomem e quais mais cresceram?
- Qual a participação de cada classe de consumo (residencial, comercial, industrial etc.)?
- Quais municípios têm maior consumo por consumidor?

## Fonte dos dados

Portal de Dados Abertos do Governo de Alagoas, conjunto "Energia Elétrica por município" (CSV):
https://dados.al.gov.br/catalogo/dataset/f0521778-ba21-4207-8b1d-b1197d3e6759/resource/9b2e41fc-2a03-412a-947b-30f265d5fac7

A base tem 26.007 registros de 102 municípios, de 2010 a 2025, com as colunas: código do município, nome do município, ano, variável, categoria, subcategoria e valor. A fonte informa que valores negativos ocorrem quando há refaturamentos maiores que os faturamentos normais.

## Tecnologias

Python, pandas, Plotly e Google Colab.

## Etapas do projeto

1. **Exploração:** conferência das colunas, do período, de nulos, duplicados e valores negativos.
2. **Limpeza:** remoção de duplicados e nulos, padronização dos nomes dos municípios e separação entre consumo e número de consumidores. Os valores negativos (refaturamento) foram removidos; no consumo, foram 8 registros.
3. **Análise:** evolução anual, ranking de municípios, crescimento entre o primeiro e o último ano, participação por classe, variação percentual anual e consumo por consumidor.
4. **Visualização:** gráficos de linha e de barras com Plotly.

## Resultados

- O consumo total passou de cerca de 2,51 milhões em 2010 para cerca de 4,94 milhões em 2025 (na unidade da fonte).
- Houve uma queda até 2019 e um salto de cerca de 24% de 2021 para 2022, que merece investigação.
- Maceió lidera o ranking, seguida por Marechal Deodoro e Arapiraca.

![Consumo total por ano](Consumo%20total%20de%20energia%20por%20ano.png)
![Ranking de municípios](Ranking%20de%20munic%C3%ADpios.png)

## Como executar

1. Baixe o CSV no portal da fonte (link acima).
2. Abra o notebook `EnergiaBR_Insights.ipynb` no Google Colab.
3. Envie o arquivo `energia-eletrica-por-municipio.csv` para o Colab (pasta `/content/`).
4. Execute as células em ordem.

## Limitações

- A base cobre apenas o estado de Alagoas.
- Os valores seguem a unidade da fonte.
- A causa do salto de 2022 não foi investigada.

## Autor

Lucas Braga Scudeler
LinkedIn: https://www.linkedin.com/in/lucas-braga-scudeler
