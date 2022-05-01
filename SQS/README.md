#### SQS (Simple Queue Service)

* Abrir o SQS -> Criar fila;
* aws configure (no cli para adicionar as credenciais);
* Default regigion: us-east-1;
* Default output formar: json;

#### ---- AWS CLI
* aws sqs help;
* aws sqs list-queues
* aws sqs send-message --queue-url https://sqs.us-east-2.amazonaws.com/500232270682/alura-teste --message-body "Olá mundo"
* aws sqs receive-message --queue-url https://sqs.us-east-2.amazonaws.com/500232270682/alura-teste
 OBS: Sugerido passar o parâmetro --wait-time-seconds com um valor maior do que 0. Isso mantem uma conexão aberta para não precisar ficar fazendo pings
* aws sqs delete-queue --queue-url https://sqs.us-east-2.amazonaws.com/500232270682/alura-teste
* aws sqs create-queue --queue-name <value>
* aws sqs delete-message --queue-url https://sqs.us-east-2.amazonaws.com/500232270682/alura-test --receipt-handle <value obtido no receive-message>

#### DLQ (Dead Letter Queue)

* Crie uma fila normal no aws, coloque o sufixo '-dlq' no nome dela só para controler;
* Vá até outra fila, e nas configurações de dlq dela aponte para a fila dlq criada anteriormente; 