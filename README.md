## Santander Challenge ##

*O Objetivo deste Challenge é criar uma topologia baseada cloud em componentes 3 camadas*

1. Camada - Entrada
   - Componentes:
     - WAF - Proteção dos dados (Web Application Firewall)
     - Load Blance
     -  Ngix - Web Server/API Gateway
   
3. Camada de Serviço
    - Serviço de Gerenciamento de Fila - Kafka MQ
   
4. Camada de Cache / Armazenamento
    - Componente
    - Redis - Cache
    - Banco de dados - PostGres


Conceito deste 
