#### Simple Storage Service (S3)

###### Buckets

* É o diretório raiz quando criamos um armazenamento com S3. Qualquer sub-diretório criado dentro deste é chamado de folder (Diretório);
* Quando um buacket é criado deve ser especificado a região que ele vai ser criado;
* Por padrão um arquivo adicionado no buacket ou diretório tem permissão pública desativa, para alterar basta acessar o arquivo, ir em permissão e editar;
* Se a configuração do bucket impedir o acesso público nenhum arquivo pode ser público;
* Se a configuração do bucket permitir o acesso público os arquivos poderão ser públicos, mas o padrão na criação de cada arquivo ainda é ser privado;
* Versionamento de objetos: Só pode ser aplicado a nívelde bucket, Bucket -> Propriedades -> Versionamento de Bucket;

###### Objects 

* São os arquivos armazenados dentro do buckets e seus sub-diretórios;
* Para alterar o ciclo de vida dos objetos (Regras de armazenamento programaticamente):  Abrir o bucket -> Gerenciamento -> Criar regra de ciclo de vida;
