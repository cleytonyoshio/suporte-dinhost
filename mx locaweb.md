## Configuração de MX, Locaweb ##

Na Zona de DNS do domínio, insira os apontamentos para o serviço de e-mail de acordo com as tabelas. Depois, aguarde a Propagação de DNS.

### Apontamentos do tipo CNAME ###
|Entrada|Tipo|Prioridade|Conteúdo
|---------------|---------------|---------------|---------------|
|pop|CNAME|0|mail.ita.locaweb.com.br|
|smtp|CNAME|0|pop.seudomínio|
|imap|CNAME|0|pop.seudomínio|
|mail|CNAME|0|pop.seudomínio|
|webmail|CNAME|0|webmail-seguro.com.br|
|calendario|CNAME|0|calendario.locaweb.com.br|
|autodiscover|CNAME|0|autodiscover.email.locaweb.com.br|


###  Apontamento do MX ###
|Entrada|Tipo|Prioridade|Conteúdo|
|---------------|---------------|---------------|---------------|
|.|MX|10|mx.a.locaweb.com.br|
|.|MX|10|mx.b.locaweb.com.br|
|.|MX|10|mx.jk.locaweb.com.br|



### Apontamento do tipo TXT ###
|Entrada|Tipo|Prioridade|Conteúdo|
|---------------|---------------|---------------|---------------|
|.|TXT|0|v=spf1 include:_spf.locaweb.com.br ?all|
