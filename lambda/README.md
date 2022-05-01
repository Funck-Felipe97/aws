#### API Gatewat

* Acessar API Gateway e criar uma API Rest (Clicar em compilar);
* Selecionar Rest e Nova API;
* Ir em ações e criar novo recurso;
* Selecionar o recurso e ir em ações e criar um método;
* Selecionar o tipo de integração (Lambda) e em função lambda escolha uma função já existente;
* É possível realizar testes pela pagina;
* Para realizar testes via url pública é necessário clicar em ações e implantar API;
* Os deploys estão na aba estágio;

###### Criando integração entre lambda e API Gateway

* Va até um endpoint no Gateway e clicar em criar integração;
* Selecione a opção de Usar a integração de proxy do Lambda;
* Isso vai fazer com que o retorno do lambda seja utilizado para montar a resposta http do gateway, exemplo, o lambda retorna um campo statusCode na resposta, isso vai se transformar no statusCode do resposta http do gatewsay. doc (https://docs.aws.amazon.com/pt_br/apigateway/latest/developerguide/set-up-lambda-proxy-integrations.html)

###### Adicionando campos obrigatórios no seu endpoint gateway

* Vá até seu endpoint e depois em solicitação de método;
* Vovê pode adicionar propriedade que seu endpoint precisa, como queryParam, pathVariable, body etc;
* Depois é necessário fazer uma nova implatação;

###### SAM Framework

* Iniciar um novo projeto
* sam init;
* sam local invoke "HelloWorldFunction"
* sam local invoke "HelloWorldFunction" -e events/event.json  // para invocar uma function passando evento
* sam local start-api // Para subir a api gateway local
* sam build && sam deploy -g  // para fazer deploy do lambda





