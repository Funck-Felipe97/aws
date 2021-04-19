#### AWS IAM (Identity Access Management)

* Controla o acesso de outros usuários a uma conta AWS;
* Um novo usuário por padrão não tem acesso nenhum;

###### MFA (Multifactor Authetication) 

* Forma de adicionar mais segurança a conta através de um token gerado em um dispositivo;
* Suas credenciais de segurança -> Ativar MFA -> Dispositivo MFA virtual;
* Aplicativo 2FAS Auth para gerar chaves

###### Novo usuário na conta;

* Usuários -> Adicionar novo usuário;
* Anexar politicas existentes de forma direta -> AdministradorAccess;
* Por ultimo adicionar tags, ex: Cargo;

###### Novo grupo  na conta;

* Grupos -> Adicionar novo grupo;
* Adicionar permissão;