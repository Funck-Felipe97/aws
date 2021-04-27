#### Simple Notification Service (SNS)

* O envio de notificações funciona com tópicos e assinates;
* Para criar um Tópico: SNS -> Dashboard -> Tópicos -> Criar novo tópico;
* Dentro do tópico é possível criar uma assinatura para ele;
* Dentro do tópico é possível enviar mensagens para os assinantes;

#### CloudWatch

* Para criar um Dashboard: CloudWatch -> Painéis -> Criar Painel;
* Na configuração do panel escolher as métricas e serviços ao criar um widgets;
* Para criar alarme: CloudWatch -> Alarmes -> Criar alarmes -> Selecionar o serviço -> Configurar quando ele deve ser disparado -> Adicionar o tópico que vai ser notificado;