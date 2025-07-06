[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gabrielsimas/clima-rj-analise/blob/master/MVP_AlertaRio.ipynb)


# MVP AlertaRio – Análise do Impacto do ENSO no Clima do Rio de Janeiro

Este projeto realiza uma **análise exploratória dos dados históricos de clima** do Rio de Janeiro (1997–2024), com ênfase no impacto do fenômeno **ENSO** (El Niño, La Niña e Neutro) sobre **temperatura** e **precipitação**. O estudo busca identificar padrões, extremos e validar premissas conhecidas da climatologia, empregando técnicas de Estatística Descritiva, limpeza e visualização de dados em Python.

## Objetivo

- Avaliar se eventos de El Niño e La Niña influenciam significativamente as médias de temperatura e episódios extremos (ondas de calor/frio e chuvas intensas) na cidade do Rio de Janeiro.
- Ilustrar graficamente as principais tendências e responder a hipóteses formuladas a partir do conhecimento meteorológico.

## Premissas e Hipóteses

1. **El Niño**: associado ao aumento das temperaturas médias e maior ocorrência de ondas de calor.
2. **La Niña**: favorece a diminuição das temperaturas médias e mais episódios de frio.
3. O ENSO pode influenciar não só temperaturas, mas também a frequência de extremos de chuva.
4. **Hipótese central**: anos de El Niño terão médias de temperatura superiores a Neutro/La Niña, enquanto anos de La Niña terão médias inferiores.

## Fontes de Dados

- **Dataset**: Histórico de clima de estações meteorológicas do AlertaRio – Rio de Janeiro (1997–2024).
- Variáveis principais: Data, Temperatura, Umidade, Acumulado de Chuva (24h), Estação, ENSO_Fase, Período do dia, Estação do ano, entre outras.

## Metodologia

- **Pré-processamento**: Checagem de valores faltantes (NaN), remoção/tratamento de outliers, padronização de colunas.
- **Análise descritiva**: Cálculo de médias, desvios, quartis, limites e identificação de extremos.
- **Visualização**: Gráficos de boxplot, barras, dispersão, heatmaps e tendências anuais.
- **Comparação**: Todos os resultados segmentados por fase do ENSO e sazonalidade.

> **Nota:** Não foi necessário utilizar técnicas de encoding para variáveis categóricas (como OneHotEncoding), pois a análise foi conduzida inteiramente por agrupamento e agregação estatística.

## Resultados

- El Niño confirmou-se associado às maiores médias e frequência de ondas de calor.
- La Niña não apresentou médias tão baixas quanto esperado, resultado influenciado pelo recorte temporal recente do fenômeno.
- Os maiores extremos de chuva variaram entre fases do ENSO e estações do ano, com maior acúmulo no verão.
- As premissas foram parcialmente validadas; o contexto do aquecimento global também se mostrou relevante.

## Como Executar

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/MVP_AlertaRio.git
