## Configuração do Outlook, servidores de e-mail ##

Clique na guia Arquivo.

Clique Configurações de Conta e clique em Configurações de Conta.

Selecione a conta de email que você deseja atualizar e clique em Alterar.

Em Informações do Servidor, na caixa Servidor de entrada de emails, digite: email.dinhost.com.br

Em Informações do Servidor, na caixa Servidor de saída de emails, digite: email.dinhost.com.br

![acessar dados da conta](https://osiprodeusodcspstoa01.blob.core.windows.net/pt-br/media/d6797029-9412-46c5-930c-c6bc8dc8f85e.jpg)

Após realizar a alteração dos servidores clique sobre o botão mais opções:

![Mais opcoes](http://wiki.locaweb.com.br/images/f/fa/3chgport_outlook.png)

Ao configurar os dados servidores de envio e recebimento nas configurações avançadas é necessário ativar as opções de criptografia SSL e autentiacação.

`
Servidor de SMTP requer autenticação e usar mesmas config. do servidor de entrada de e-mails.
`

![Ativando Autencicação smtp](http://wiki.locaweb.com.br/images/2/24/06_m.jpg)


``
Dados inseridos na aba Avançado de configuração do e-mail
``

O servidor de entrada pode ser do tipo **POP** ou **IMAP**:
- POP - Host: email.dinhost.com.br / Segurança: SSL / Porta: 995
- IMAP - Host: email.dinhost.com.br / Segurança: SSL / Porta: 993

Dados do servidor de saída **(SMTP)**:
- SMTP - Host: email.dinhost.com.br / Segurança: SSL / Porta: 465
