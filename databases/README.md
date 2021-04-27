#### Relational Database Service (RDS)

* Instâncias RDS devem estar em subredes privadas por questões de segurança;
* O banco é acessado através de uma instância EC2 que esta em uma subrede publica;
* No EC2 executar: `sudo apt install postgresql-client-common postgresql-client -y` para instalar o client do postgres

###### Criando um banco

* AWS -> RDS;
* Criar um subnet group em subnet groups;
* Vincular o grupo a uma subrede privada;
* Criar uma database em Dashboard;
* Liberar o acesso externo a base: Selecionar a database -> Security groups rules -> editar regras de entrada -> Liberar o acesso de qualquer ip;
* Para conectar via psql: `psql -h database-1.ckkz4j4ckakf.sa-east-1.rds.amazonaws.com -U postgres -W`