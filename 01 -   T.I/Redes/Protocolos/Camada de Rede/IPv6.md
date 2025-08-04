
# IPv6


## Endereçamento

Possibilidade de endereçamento público para todos os dispositivos da Internet

Utiliza 128 bits e não mais 32 bits

Escritos em formato HEXADECIMAL

A cada 4 bits gera-se um algarismo HEXADECIMAL

Criam-se 8 blocos de 4 algarismos HEXADECIMAIS 000 a FFFF

0’s à esquerda podem ser suprimidos em um mesmo bloco

Sequências de 0’s em blocos distintos podem ser agrupados (<font color="#d99694">apenas uma vez por endereçamento</font>)


![[Pasted image 20250723172931.png]]



## Endereços reservados:

<font color="#4bacc6">Endereços Multicast </font>→ São estruturados por FF00::/8

<font color="#4bacc6">Endereços de Loopback</font> → 0:0:0:0:0:0:0:1 ou ::1

<font color="#4bacc6">Transição 6to4</font> → 2002::/16

<font color="#4bacc6">Transição Teredo</font> → 2001::/32



![[Pasted image 20250723173142.png]]



## Mapeamento de Endereço IPv4

::FFFF:wxyz, onde wxyz representa os 32 bits do endereço IPv4

NAT64 → prefixo 64:ff96::/96



## Cabeçalho

Tamanho fixado em 40 bytes

Quantidade menor em campos do que o IPv4

<font color="#4bacc6">Classe de Tráfego</font> → 8 bits. Função similar ao de ToS do IPv4

<font color="#4bacc6">Identificação de Fluxo</font> → 20 bits. Marcação de tráfego. Foi criado para suporte à QoS

<font color="#4bacc6">Tamanho do campo de dados</font> → 16 bits, indicando o tamanho <font color="#c0504d">APENAS dos dados enviados junto ao cabeçalho</font>

<font color="#4bacc6">Próximo cabeçalho</font> → 8 bits. Referencia os cabeçalhos de extensão eventualmente utilizados. Caso não haja, consta a informação do protocolo da camada superior

<font color="#4bacc6">Limite de Salto</font> → 8 bits. Campo similiar ao TTL do IPv4, determinando o tempo de vida ou limites de saltos do pacote de rede

<font color="#4bacc6">Endereços de Origem e Destino</font> → Define os endereços de 128 bits de origem e destino dos pacotes IPv6


![[Pasted image 20250724111038.png]]


## Cabeçalhos de entensão

Hop-by-hop (00)

Destination Options (60)

Routing (43)

Fragmentation (44)

Authentication Header (51)

Encapsulation Security Payload (50)


## Novidades

- <u>IPSeC</u> é obrigatório

- <u>Jumbograms</u> (pacotes maiores do que 64Kb - antes era limitados no IPv4)

- Fragmentação não ocorre nos <u>nós intermediários</u>, somente na origem.



## Tipos de encaminhamento

- Unicast

- Anycast → com métricas específicas

- Multicast


## Protocolos Auxiliares

[[DHCPv6]]

[[ICMPv6]]

[[RS e RA]]

[[NS e NA]]


## Tráfego controlado por congestionamento

Os pacotes são retirados da rede quando o índice de utilização do canal está muito alto.
Possui 7 níveis de prioridade


## Tráfego não controlado por congestionamento

Este se refere a um tipo de tráfego com expectativa de atraso mínimo. A eliminação de pacotes é indesejável.
Níveis de prioridade de 8 a 15

![[Pasted image 20250724122911.png]]


## Técnicas de Transição

**Statefull** → Necessário manter tabelas de estado com informações sobre os endereços com pacotes para processá-los

**Stateless** → Cada pacote é tratado de forma independente



Túneis IPv4 dentro de IPv6 devem ser preferidos em detrimento de túneis IPv6 sobre IPv4.

**PILHA DUPLA** → Consiste na convivência do IPv4 e do IPv6 nos mesmos equipamentos.
<font color="#c0504d">Essa é a técnica padrão para a transição para IPv6</font>

**TÚNEIS** → Diferentes redes IPv4 comuniquem-se através de uma rede IPv6, ou vice-versa

**TRADUÇÃO** → Equipamentos IPv6 comuniquem-se com outros que usam IPv4, por meio de conversão dos pacotes


### Pilha Dupla

Deve-se configurar toda a arquitetura de Rede para os dois contextos

Implementar o DNS com registros do tipo AAAA (quad A)

Preferência dada ao IPv6


### Túneis 6over4 (IPv6 - over - IPv4)

Faz-se o encapsulamento de pacotes IPv6 em pacotes IPv4

Adequar os endereços de origem e destino para o IPv4 e colocar no cabeçalho o tipo 41 (29 em hexadecimal), também conhecido como protocolo 41

No destino, quando receber o tipo 41, a máquina remove o cabeçalho IPv4 e interpreta o cabeçalho IPv6

Do mesmo modo, é possível encapsular pacotes IPv6


### Tunnel Broker


### NAT444 ou Longe Scale Nat ou GCN



### NAT64 e DNS64


### 6to4


### Teredo








