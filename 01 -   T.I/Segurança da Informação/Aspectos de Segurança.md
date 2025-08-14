
# Aspectos de Segurança - Email

## Spoofing de e-mail

Utilização de um nome falso ou de propriedade para envio da mensagem (Altera-se ou se manipula o campo “<u>MAIL FROM</u>“)

## PGP

Utilizado em ambientes simples e menos formais. Utilização e implementação da assinatura digital e criptografia da mensagem.

## S/MIME

Adiciona **criptografia** e **assinatura digital** ao MIME, garantindo **confidencialidade**, **integridade** e **autenticidade** das mensagens e anexos. Foco de utilização em ambientes complexos e corporativos.

## TÉCNICA SPF (Sender Polity Framework)

Foca na atuação sobre o spoofing de e-mail. Busca <u>garantir a legitimidade do remetente.</u>


## TÉCNICA DKIM (Domains Keys Identified Email)

Diferentemente do SPF, essa técnica <font color="#c0504d">verifica também o cabeçalho e o conteúdo.</font>


## DMARC (Domain-based Message Authentication, Reporting e Conformance)

Alternativa ao <u>ANTISPAM tradicional</u>. Funciona em conjunto com <u>o SPF e DKIM</u> para v<u>erificar a autenticidade do remetente e proteger contra phishing e outras ameaças.</u>

