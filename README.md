# teste-std
## Santander Challenge. ##

*O Objetivo deste Challenge é validar uma topologia baseada cloud em componentes 3 camadas*

1. Camada - Entrada
   Componentes
   WAF - Proteção dos dados (Web Application Firewall)
   Load Blance
   Ngix - Web Server/API Gateway
   
2. Camada - Damada de Serviço
    Serviço de Gerenciamento de Fila - Kafka MQ
   
3. Camada de Cache / Armazenamento
    Componente - Redis
    Banco de dados - PostGres
   
