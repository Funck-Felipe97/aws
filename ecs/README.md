#### AWS ECS (Elastic Container Service)

* Um cluster ECS é composto por 4 partes (imagem, task, service e cluster)
  * Imagem -> Define qual imagem do docker estará rodando;
  * Task -> Passa os parâmetros para a imagem, quantidade de memória, cpu etc;
  * Service -> Controla as taks, quantas task serão executadas no cluster;
  * Cluster -> Utilizar máquina para rodar a aplicação

* AWS ECS CLI
  *  aws ecs list-clusters
  *  aws ecs list-services
  *  aws ecs list-services --cluster default
  *  aws ecs list-tasks
  *  aws ecs list-tasks --service <service-name>
  *  aws ecs update-service --service sample-app-service --desired-count 0  // Atualizar parâmetro do service