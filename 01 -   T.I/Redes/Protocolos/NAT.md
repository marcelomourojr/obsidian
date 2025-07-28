
# NAT

Atuação subsidiária como recurso de segurança

Criado como solução para o esgotamento de endereços IPv4. (Porém ainda se esgotam)

Conversão de um endereço em outro 

Não há obrigatoriedade de conversão de endereço privado para público, ou, vice-versa


## Operação

- Alteração dos cabeçalhos IP

- Caso haja alteração da porta, também altera-se o cabeçalho TCP/UDP


## Tipos de NAT

1:1

N:1 (PAT; NAT OVERLOAD; NAPT)

N:M


## PAT

- Utiliza-se de portas da camada de transporte para diferenciação das conexões

## NAT Reverso

- Conexão originada do “mundo exterior“; Aplicação do conceito de balanceamento de carga

## Twice NAT (2x NAT)

- Compartilhamento de endereços públicos 

## NAT - PT

- Conversão de diferentes protocolos, como de IPv6 para IPv4