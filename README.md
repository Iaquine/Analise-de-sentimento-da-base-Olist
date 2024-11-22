# Analise de sentimentos da base Olist
# Classificação de Sentimentos em Textos com Redes Neurais Recorrentes

Este projeto utiliza Redes Neurais Recorrentes (RNNs) para classificar o sentimento em avaliações de clientes de um e-commerce brasileiro.

## Descrição do Dataset

Este dataset contém informações sobre as avaliações de clientes em uma plataforma de e-commerce brasileira. Ele faz parte do **Olist**, uma plataforma de marketplace que conecta vendedores e compradores em diversas categorias de produtos. O dataset foi coletado de transações reais e inclui avaliações de produtos e do serviço de entrega.

O dataset é ideal para análise de sentimentos, modelos de previsão de satisfação do cliente, e análise exploratória de dados. Ele fornece dados sobre os clientes, os produtos comprados e o feedback fornecido pelos consumidores após a conclusão de suas compras.

## Fonte dos Dados

Os dados estão disponíveis através do Kaggle no link: [Olist Brazilian Ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

## Arquivo CSV

- **olist_order_reviews_dataset.csv**: Este arquivo contém as informações de avaliação dos pedidos feitas pelos clientes.

## Estrutura do Dataset

O arquivo CSV contém as seguintes colunas:

1. **review_id**: ID único da avaliação do pedido.
2. **order_id**: ID do pedido ao qual a avaliação pertence.
3. **review_score**: Nota da avaliação (de 1 a 5).
4. **review_comment_title**: Título do comentário da avaliação.
5. **review_comment_message**: Mensagem do comentário da avaliação.
6. **review_creation_date**: Data de criação da avaliação.
7. **review_answer_timestamp**: Data e hora da resposta da avaliação.

## Detalhes das Colunas

- **review_id**: Identificador único para cada avaliação de pedido. É útil para rastrear avaliações individuais.
  
- **order_id**: Identificador do pedido ao qual a avaliação está associada. Isso conecta a avaliação aos detalhes do pedido e ao cliente.
  
- **review_score**: A pontuação da avaliação fornecida pelo cliente, em uma escala de 1 a 5, onde:
  - 1: Muito insatisfeito
  - 2: Insatisfeito
  - 3: Neutro
  - 4: Satisfeito
  - 5: Muito satisfeito
  
- **review_comment_title**: Título do comentário de avaliação fornecido pelo cliente, se presente.

- **review_comment_message**: Texto completo da avaliação ou feedback do cliente, onde ele pode expressar sua satisfação ou insatisfação com o produto ou serviço.

- **review_creation_date**: A data em que a avaliação foi criada.

- **review_answer_timestamp**: A data e hora em que a avaliação foi respondida (se aplicável).


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
