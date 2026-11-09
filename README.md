# Painel de Consumo de Energia Elétrica em Alagoas (2010–2025)

Análise de dados públicos sobre o consumo de energia elétrica por município e por classe de consumo em Alagoas, com gráficos que mostram a evolução, os municípios que mais consomem e o consumo por consumidor.

## Objetivo

Transformar uma base pública extensa em informações fáceis de entender, respondendo:

- Como o consumo total de energia evoluiu ao longo dos anos?
- Quais municípios mais consomem e quais mais cresceram?
- Qual a participação de cada classe de consumo (residencial, comercial, industrial etc.)?
- Quais municípios têm maior consumo por consumidor?

## Fonte dos dados

Portal de Dados Abertos do Governo de Alagoas, conjunto "Energia Elétrica por município" (CSV).
https://dados.al.gov.br/catalogo/dataset/f0521778-ba21-4207-8b1d-b1197d3e6759/resource/9b2e41fc-2a03-412a-947b-30f265d5fac7

A base tem as colunas: código do município, nome do município, ano, variável, categoria, subcategoria e valor. A fonte informa que valores negativos ocorrem quando há refaturamentos maiores que os faturamentos normais.

## Tecnologias

Python, pandas, Plotly e Google Colab.

## Etapas do projeto

1. **Exploração:** conferência das colunas, período, nulos e duplicados.
2. **Limpeza:** remoção de duplicados e nulos, padronização dos nomes de municípios, separação entre consumo e número de consumidores, tratamento dos valores negativos [explique aqui o que você decidiu fazer e por quê].
3. **Análise:** evolução anual, ranking de municípios, crescimento, participação por classe, variação percentual e consumo por consumidor.
4. **Visualização:** gráficos de linha e de barras com Plotly.

## Como executar

1. Abra o notebook `analise_energia_alagoas.ipynb` no Google Colab.
2. Execute as células em ordem. A primeira célula carrega os dados direto do portal.
3. Se o link de download não funcionar, baixe o CSV pela página da fonte e envie para o Colab.

## Limitações

- A base cobre apenas o estado de Alagoas.
- [Se aplicável: unidade de medida e como os negativos foram tratados.]

## Autor

Lucas Braga Scudeler
LinkedIn: https://www.linkedin.com/in/lucas-braga-scudeler
