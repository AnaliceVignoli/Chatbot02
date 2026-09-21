# Chatbot02

## O que foi adicionado

1. Mais exemplos no dataset de treinamento

Foram incluídas 20 novas frases distribuídas entre as intenções saudacao, preco, estoque e pedido, com o objetivo de deixar o modelo mais variado.

Antes da atividade: accuracy de 85,7%
Meio da atividade: accuracy de 83,3%

2. Nova intenção: devolucao

Adicionada uma nova classe de intenção para lidar com pedidos de troca/devolução, incluindo:

* Novos exemplos de frases no dataset
* Nova entrada no dicionário respostas, com mensagens específicas para essa intenção

Após reforço com mais exemplos, a accuracy geral do modelo subiu para 100%.

3. Extração de produto/marca

Criada a função extrair_produto, que identifica marcas conhecidas (Dell, Samsung, Apple, etc.) dentro da mensagem do usuário usando comparação simples de texto, assim como extrair_pedido. A função chatbot foi atualizada para incluir o campo "produto" no resultado retornado, junto com mensagem, intencao e resposta.
