# Analise de sentimentos da base Olist
# Classificação de Sentimentos em Textos com Redes Neurais Recorrentes

Este projeto utiliza Redes Neurais Recorrentes (RNNs) para classificar o sentimento em avaliações de clientes de um e-commerce brasileiro.

## Dados

Os dados utilizados neste projeto são provenientes do conjunto de dados "Brazilian E-Commerce Public Dataset by Olist" disponível no Kaggle:

https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?select=olist_order_reviews_dataset.csv

## Pré-processamento dos Dados

O pré-processamento dos dados inclui as seguintes etapas:

1.  Remover caracteres especiais
2.  Converter o texto para minúsculas
3.  Aplicar stemming (opcional)
4.  Remover stop words (opcional)

## Modelagem

Os seguintes tipos de modelos RNN são utilizados:

*   LSTM
*   GRU
*   Stacked LSTM

Os hiperparâmetros dos modelos são ajustados usando o Hyperband.

## Avaliação

Os modelos são avaliados com base nas seguintes métricas:

*   Acurácia
*   Precisão
*   Recall
*   F1-score
*   AUC-ROC

## Resultados

Os resultados da avaliação dos modelos são apresentados em gráficos de barras para cada métrica.

## Conclusões

O projeto demonstra como utilizar RNNs para classificar sentimentos em textos. Os resultados mostram que as RNNs podem alcançar um bom desempenho nesta tarefa.
