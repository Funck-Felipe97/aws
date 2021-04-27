#### Conectar a uma instância EC2

* `ssh -i "ServidorWEB.pem" ubuntu@ec2-54-233-222-29.sa-east-1.compute.amazonaws.com`;
* `scp -i "ServidorWEB.pem" stack.yml ubuntu@ec2-54-233-222-29.sa-east-1.compute.amazonaws.com:/home/ubuntu`;

#### Instalar o docker no Ubuntu;

* Primeiro, atualize sua lista existente de pacotes `sudo apt update`;
* Em seguida, instale alguns pacotes pré-requisito que deixam o apt usar pacotes pelo HTTPS: `sudo apt install apt-transport-https ca-certificates curl software-properties-common`;
* Então, adicione a chave GPG para o repositório oficial do Docker no seu sistema: `curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -`;
* Adicione o repositório do Docker às fontes do APT: `sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu focal stable"`;
* Em seguida, atualize o banco de dados do pacote com os pacotes do Docker do recém adicionado repositório: `sudo apt update`;
* Certifique-se de que você está prestes a instalar do repositório do Docker ao invés do repositório padrão do Ubuntu: `apt-cache policy docker-ce`;
* Finalmente, instale o Docker: `sudo apt install docker-ce`;

#### Instalar o docker-compose 

* `sudo curl -L "https://github.com/docker/compose/releases/download/1.26.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose`;
* `sudo chmod +x /usr/local/bin/docker-compose`;
* `docker-compose --version`;