## Configuração de MX, google ##

Ao configurar o uso do servidor de e-mail da google devemos alterar:
1. [CNAME](https://support.google.com/a/answer/112038?vid=1-635769016297302023-1203656616)
1. [MX](https://support.google.com/a/answer/174125?vid=1-635769016297302023-1203656616)
1. [TXT/SPF](https://support.google.com/a/answer/4568483?hl=en&ref_topic=2759192&vid=1-635769016297302023-1203656616)

### CNAME ###
|Nome/Host/Alias|TTL* (Time to Live) ou vida útil|Tipo de registro|Prioridade|Valor/Resposta/Destino|
|---------------|---------------|---------------|---------------|---------------|
|mail|3600|CNAME|1|ghs.googlehosted.com|
|webmail|3600|CNAME|5|ghs.googlehosted.com|


### MX ###
|Nome/Host/Alias|TTL* (Time to Live) ou vida útil|Tipo de registro|Prioridade|Valor/Resposta/Destino|
|---------------|---------------|---------------|---------------|---------------|
|Em branco ou @|3600|MX|1|ASPMX.L.GOOGLE.COM|
|Em branco ou @|3600|MX|5|ALT1.ASPMX.L.GOOGLE.COM|
|Em branco ou @|3600|MX|5|ALT2.ASPMX.L.GOOGLE.COM|
|Em branco ou @|3600|MX|10|ALT3.ASPMX.L.GOOGLE.COM|
|Em branco ou @|3600|MX|10|ALT4.ASPMX.L.GOOGLE.COM|

### TXT ###
|Nome/Host/Alias|TTL* (Time to Live) ou vida útil|Tipo de registro|Prioridade|Valor/Resposta/Destino|
|---------------|---------------|---------------|---------------|---------------|
|||TXT|| v=spf1 include:_spf.google.com ~all|


