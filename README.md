# Assistente de Delivery

🏷️ **Descrição**
O projeto "Assistente de Delivery" é uma solução automatizada que utiliza **AWS Step Functions** e **Amazon Bedrock** para gerenciar e otimizar o fluxo de pedidos de delivery. O objetivo é criar um assistente que coordene tarefas desde a recepção do pedido até a entrega final, proporcionando uma experiência personalizada e eficiente ao cliente.

## Índice
- [Introdução](#introdução)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Fluxo de Trabalho](#fluxo-de-trabalho)
- [Como Funciona](#como-funciona)
- [Implantação](#implantação)
- [Logs e Monitoramento](#logs-e-monitoramento)
- [Contribuição](#contribuição)
- [Licença](#licença)

## Introdução
Este projeto foi desenvolvido com o intuito de facilitar o gerenciamento de pedidos de delivery por meio da automação. A utilização de **AWS Step Functions** permite orquestrar diferentes serviços da AWS para validar pedidos, processar pagamentos e atualizar status, enquanto o **Amazon Bedrock** oferece recursos de inteligência artificial para personalização.

## Tecnologias Utilizadas
- **AWS Step Functions**: Orquestração de serviços da AWS.
- **Amazon Bedrock**: Inteligência artificial para personalização.
- **Amazon API Gateway**: Exposição da API para recepção de pedidos.
- **AWS Lambda**: Execução de funções para validação e processamento.
- **Amazon DynamoDB**: Armazenamento de dados dos pedidos.
- **Amazon SNS**: Notificações em tempo real.
- **Amazon S3**: Armazenamento de logs e dados.

## Fluxo de Trabalho
O assistente de delivery segue o seguinte fluxo de trabalho:

1. **Recepção do Pedido**: O cliente realiza um pedido através da API.
2. **Validação do Pedido**: O sistema valida as informações do pedido.
3. **Processamento de Pagamento**: O pagamento é processado via serviço de pagamento.
4. **Atualização de Status**: O status do pedido é atualizado no banco de dados.
5. **Notificação ao Cliente**: O cliente é notificado sobre o status do pedido.
6. **Preparação do Pedido**: O pedido é preparado para entrega.
7. **Entrega do Pedido**: O pedido é marcado como entregue após ser recebido.

## Como Funciona
1. **Recepção do Pedido**: O pedido é recebido através do **API Gateway** e armazenado no **DynamoDB**.
2. **Validação e Processamento**: As funções **AWS Lambda** realizam a validação do pedido e o processamento do pagamento.
3. **Atualização e Notificação**: O status do pedido é atualizado e o cliente é notificado através do **Amazon SNS**.
4. **Armazenamento de Dados**: Todos os dados são armazenados no **Amazon S3** para análise futura.

## Implantação
Para implantar o assistente de delivery, siga estas etapas:
1. **Configuração do Ambiente**: Configure sua conta AWS e ative os serviços necessários.
2. **Criação de Recursos**: Crie os recursos no AWS como Lambda, DynamoDB, API Gateway, etc.
3. **Deploy da Aplicação**: Utilize o AWS Management Console ou AWS CLI para fazer o deploy.
4. **Teste o Sistema**: Realize testes para garantir que o fluxo de trabalho funcione conforme esperado.

## Logs e Monitoramento
Os logs são armazenados no **Amazon S3** com um nível de log configurado como `INFO`. Isso permite que você monitore a operação do assistente e identifique quaisquer problemas.

## Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias ou correções.

## Licença
Este projeto é licenciado sob a [MIT License](LICENSE).

