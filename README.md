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
    - Componentes:
       - Redis - Cache
       - Banco de dados - PostGres

------------------------

Conceito desta topolgia foi criar uma topologia em três camadas, onde cada camada ou resource group, tem sua proteção em um network securitu group, aceitando suas conexões somente na porta padrão dentro de cada endpoint em seu respectivo link.
Foi colocado a entrada dos dados via API em alta disponibidade e os demais serviços sem a mesma caracteristica.


[Para o HLD Acesse](https://drive.google.com/file/d/1WbQtBnFG3fHTw6z822RRP2L9axZZKo8c/view?usp=drive_link)
