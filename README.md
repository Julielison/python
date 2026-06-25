# gRPC Python Client - Order Service

Este repositório contém a implementação de um cliente gRPC em Python para se comunicar com o microsserviço de gerenciamento de pedidos (Order Service). O projeto foi desenvolvido usando Protocol Buffers (v3) e gRPC.

## Pré-requisitos

Antes de executar o projeto, você precisa ter:

- Python 3.8+
- pip

## Instalação

1. Clone o repositório e entre na pasta do projeto.
2. Instale as dependências:

pip install -r requirements.txt

## Executando o cliente

O arquivo principal é o client.py.

Ele cria uma requisição simulada com itens de pedido e envia para o servidor gRPC usando insecure_channel no endereço localhost:3000.

Para executar:

python client.py

## Estrutura dos arquivos gerados

- order_pb2.py: mensagens geradas pelo Protocol Buffers (CreateOrderRequest, OrderItem, CreateOrderResponse)
- order_pb2_grpc.py: stubs gRPC usados pelo cliente (OrderStub)
