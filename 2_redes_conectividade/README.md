###### Virtual Private Cloud (VPC)

###### Gateway

* Se tivermos recursos criados na nossa VPC como uma máquina virtual (EC2), banco de dados 
(RDS) etc, não é possível desconectar a VPC do Intenert Gateway

###### Tabela de rotas (Route tables)

###### Lista de controle de acesso a internet (Network ACLs)

* Funciona como um firewall e controle o acesso de enterda e saida das subnets

###### Subnets

* Subnets  são redes localizadas em uma zona de disponibilidade;
* Por padrão uma sub-rede esta associada a tabela de rotas padrão;
* Para deixar uma subede privada basta associar a uma tabela de rotas sem acesso a internet;
* Para deixar uma subrede pública basta deixar associada a uma tabela de rotas com acesso a internet