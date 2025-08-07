
# Protocolos de Correio Eletronico

Principais elementos: MUA e MTA

<font color="#4bacc6">MUA</font> → Mail User Agent (comunicação entre cliente e servidor)

<font color="#4bacc6">MTA</font> → Mail Transfer Agent (Intermediário para envio e recebimento das mensagens)

Permite a troca de mensagens eletrônicas de forma assíncrona


## SMTP

Responsável <font color="#c0504d">pelo envio da informação</font>

Atua na porta <font color="#c0504d">25/TCP</font>. Na versão segura <font color="#c0504d">SMTPS na porta 465</font>

<font color="#c0504d">Não implementa de forma nativa</font> recursos de segurança


## POP3

Atua na porta 110/TCP. Na versão segura POPS na porta 995

Efetua o download das mensagens para o dispositivo de acesso

- Mensagem removida do servidor


## IMAP

Atua na camada de aplicação na <font color="#c0504d">porta 143/TCP</font>. Na versão segura <font color="#c0504d">IMAPS na porta 993</font>

<font color="#c0504d">Gerência das mensagens ocorre de forma online diretamente no servidor MTA</font>




![[Pasted image 20250805141336.png]]


