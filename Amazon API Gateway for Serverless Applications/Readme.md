O API Gateway é um serviço que facilita a criação, a publicação, a manutenção, o monitoramento e a segurança de suas APIs em qualquer escala. 

exemplos de uso:
API do Escritório de meteorologia
imagem 02.png

API do provedor de identidade social
coisas.png

Recursos do desenvolvedor no API Gateway
- Executar várias versoes de uma API ao mesmo tempo.
- Geracao rápida de SDKs
-Transformar ou validar dados de solicitação/resposta
Recursos para gerenciar acesso a APIs
- Reduzir latencias e limitar o tráfego
- Opcoes de autorizacao integradas e flexíveis
chaves de API para desenvolvedores externos

Arquitetura do API Gateway
um exmplo de um visao geral dos conteios e recusos do uso da API gatway

gatway.png
Opcoes para criar tipos de apis:
API REST
API HTTP
API WEBSOCKET

Amazon API Gateway for Serverless Applications


Hugo lemos
  10h09
AWS Lambda é um serviço computacional sem servidor, orientado a eventos, que lhe permite executar código sem provisionar nem gerenciar servidores.


Hugo lemos
  15h52
Arquiteturas orientadas a eventos
Uma arquitetura orientada a eventos usa eventos para iniciar ações e comunicação entre serviços desacoplados.
O que é uma função do Lambda?
O código executado no AWS Lambda é chamado de função do Lambda.
As funções do Lambda são stateless, sem afinidade com a infraestrutura subjacente.
Como o AWS Lambda funciona
As fontes de eventos podem invocar uma função do Lambda em três padrões gerais. Esses padrões são chamados de modelos de invocação.
Invocação síncrona
basicamente o Lambda executa a função e aguarda uma resposta. não há novas tentativas internas.  Os seguintes serviços da AWS invocam o Lambda de maneira síncrona:
Amazon API Gateway
Amazon Cognito
AWS CloudFormation
Amazon Alexa
Amazon Lex
Amazon CloudFront
Invocação assíncrona
os eventos são enfileirados e o solicitante não aguarda a conclusão da função. Esse modelo é indicado quando o cliente não precisa de uma resposta imediata.
Os seguintes serviços da AWS invocam o Lambda de maneira assíncrona:
Amazon SNS
Amazon S3
Amazon EventBridge
Invocação de sondagem
foi projetado para se integrar aos serviços baseados em streaming e enfileiramento da AWS sem gerenciamento de código ou servidor.
Esse modelo de invocação dará suporte aos seguintes serviços:
Amazon Kinesis
Amazon SQS
Amazon DynamoDB Streams
A configuração de serviços como gatilhos de eventos é conhecida como mapeamento da fonte de eventos. Esse processo ocorre quando você configura fontes de eventos para executar as funções do Lambda e, em seguida, concede a essas fontes permissões do IAM para acessar a função do Lambda.
O Lambda lê eventos dos seguintes serviços:
Amazon DynamoDB
Amazon Kinesis
Amazon MQ
Amazon Managed Streaming for Apache Kafka (MSK)
Apache Kafka autogerenciado
Amazon SQS
Comportamento de erro do modelo de invocação
fazer o quadro.


Hugo lemos
  0h34
Designing Event-Driven Architectures