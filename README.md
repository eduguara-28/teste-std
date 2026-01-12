# teste-std
## Santander Challenge ##

*O Objetivo deste Challenge é validar uma topologia baseada cloud em componentes 3 camadas*

1. Camada - Entrada
   - Componentes
   -- WAF - Proteção dos dados (Web Application Firewall)
   -- Load Blance
   -- Ngix - Web Server/API Gateway
   
3. Camada - Damada de Serviço
    - Serviço de Gerenciamento de Fila - Kafka MQ
   
4. Camada de Cache / Armazenamento
    - Componente
    -- Redis - Cache
    -- Banco de dados - PostGres
   
