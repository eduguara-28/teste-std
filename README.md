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


--------------------------

 Para a parte 2 do teste, criei com a ajuda do copilot o playbook de instalação dos pacotes acima mencionados usando componentes acima mencionados, arquivo install.yml.
 Acredito para um bom funcinamento do playbook alem de estar escrito corretamente é a anotação da estrutura da pasta em cada playbook, conforme a propia indicação da redhat, sem esta, existe grande changes do playbook funcionar de uma maneira errática ou mesmo com dificuldades de compartilhar o código.
 [documentação referencia](https://docs.ansible.com/projects/ansible/latest/dev_guide/developing_collections_structure.html)
 
├── playbooks/

│   ├── files/

│   ├── vars/

│   ├── templates/

│   └── tasks/


Um ultimo detalhe porem não menos importante é ter um inventário, um destino correto onde este script será executado, assim, evitando uma execução erronea ou mesmo problemas de deploy em equipamentos que não fazem parte do escopo.
