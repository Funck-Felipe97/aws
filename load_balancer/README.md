#### Elastic Load Balancer (ELB)

* A função do ELB é somente balancear cargas;
* Um novo ELB pode ser criado em ECS -> Balanceamento de carga -> Load Balancers;
* Colocar o load balancer em sub rede pública;

#### Auto Scaling

* Scala os servidores conforme a necessidade, tanto para mais quanto para menos;
* ECS -> Instâncias -> Modelos de execução -> Criar modelo de execução;
* Habilitar o auto scaling na configuração;
* Selecionar a mesma imagem e tipo de instância do serviço que vc deseja escalar;
* Configurações de rede -> Selecionar EC2 - Classic;
* Em dados do usuário inserir script para inicializar o servidor web;

----------

* Ir em auto Scaling -> Grupos Auto Scaling
* Etapa 1 -> Vincular ao modelo de execução criado anteriormente;
* Etapa 2 -> Selecionar rede pública;
* Etapa 3 -> Habilitar balancemaneto de carga, escolher grupo de destino para o load balancer;
* Etapa 4 -> Configurar o mínimo, máximo e desejável de instâncias. Confiurar pólica para escalar, ex: Consumo de CPU;



