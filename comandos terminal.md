## Comandos Terminal Copiar sites de outro servidor ##

- **Acesso ao servidor plesk por ssh**
ssh user@dominio
- **Abrindo pasta com os sites no servidor**
cd /var/www/vhosts

- **Limpando todo conteúdo da pasta httpdocs atual**
rm -rcf *

- **Copia os dados de outro servidor para este**
scp -r (servidor de origem) ./
``
sendo servidor de origem (root@dominio:caminho da pasta)
``
- **Entrar com outro usuario**
su + [nome do usuario]

## Copiar em segundo plano ##
- **screem -r (nome do terminal)**
``
Comando abre uma nova pagina do terminal em permite deixa-la executando em segundo plano.
``

ctrl + a, segura ctrl e aperta d para minimizar e retomar o comando para abrir novamente.

## Permissão para arquivos ##
- **chown [novo proprietário] [caminho/da/pasta/arquivo] [-R]**
``
Altera o nome do proprietário.
``

- **chmod +rwx**
``
Sendo as permissões: +r leitura, +w escrita, +x execução
``
Para retirar a permissão utilizar -r-w-x

- **chgrp [novo grupo] [caminho/pasta/arquivo] [-R]**
Altera o nome do grupo ou caminho para onde este aponta.

##dump my sql##
- **mysqldump -h dominio -u (user) -p(pass) eschema > dump.sql**
- **mysql -u (user) -p(pass) dominio < dump.sql**
