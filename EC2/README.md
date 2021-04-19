#### Elastic Cloud Computer (EC2)

* AMI (Amazon machine image): Uma imagem da Amazon é um pacote de cplicação pré-configurado para instâncias EC2 que incluem um sistema operacional, outras aplicações e configurações padrão;


##### Criando uma nova instância EC2

* Executar instância -> Executar Instância;
* Selecionar a imagem que será instalada na instância;
* Escolher o tipo de instância (Memória, CPU, Armazenamento etc);
* Configurar instância -> Deixar configurações default (Nesta etapa é possível definir qual sub-rede da instância além de rodar script no campo user data);
* Configurar os volumes e espaços de armazenamento;
* Adicionar tags;
* Adicionar regras de segurança em Configure Security Group (Ex: Habilitar ssh, http, requisições de qualquer ip ou um ip especifico);

###### Elastic Block Store (EBS)

* É um volume de armazenamento para uma instância EC2, ou seja, algo como o disco rígido da máquina virtual;

###### IOPS - Input/Output Operations per Second

* A quantidade de dados que podem ser lidos ou escritos em um voume EBS por segundo

###### Snapshot

* É um backup ou fotografia de um determiando momento de um volume. Pode ser usado como basse na criação de novos volumes;

###### Grupo de segurança

* De forma simples, Security Groups são muito similares ao NACL. Ou seja, fazemos use de grupos de segurança nós podemos permitir ou negar tráfego, mas neste caso fazemos isso em nível de instância do EC2