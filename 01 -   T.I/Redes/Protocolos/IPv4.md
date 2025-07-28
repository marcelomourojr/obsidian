# IPv4

Utiliza como critério de entrega a técnica de melhor esforço

## Cabeçalho

![[Pasted image 20250714154101.png]]

Variável: 20 a 60 bytes

### VER - Version (4bits)

- Primeiro campo a ser lido e informa a versão do protocolo IP utilizado.


### IHL - Information Header Lenght (4 bits)

- Define o tamanho do cabeçalho e informa a quantidade de palavras de 32 bits


### Service Type ou TOS (Type of Service) (8 bits)

- Aplicado para fins de QoS. Possível tratar aspectos de confiabilidade e velocidade de tráfego. Atualmente definido como DSCP. Utiliza 6 dos 8 bits

### Total Length (16 bits)

- Define o tamanho total do datagrama IP (Cabeçalho + Dados)

- Pode variar de 20 bytes a 65.535 bytes 

- Para saber o tamanho do conteúdo, deve-se descontar o IHL


### Identifier (16 bits)

- Campo de identificação do pacote IP. Utilizado para fins de Fragmentação


### Fragment Offset (13 bits)

- Utilizado para definir o sequenciamento/posicionamento dos fragmentos


### Flags (3 bits)

- 1 - bit: Reservado
- 2 - bit (DF - Dont Fragment) - Indica que o pacote não deve ser fragmentado
- 3 - bit (MF - More Fragment) - Indica que há mais fragmentos para completar o original


### Time to Live - TTL (8 bits)

- Determina o tempo de vida do pacote de rede. É mapeado a partir da quantidade de salto


### Protocol (8 bits)

- Possibilita definir o protocolo utilizado na camada superior ou na própria camada


### Header Checksum (16 bits)

- Utiliza um algoritmo sobre todo o cabeçalho IP para validar sua integridade

- Não alcança os dados ou payload

- Deve-se recalcular esse campo em cada salto


### Source and Destination Address (32 bits)

- Destinado aos endereços IP de origem e destino


### Options and Padding (Tamanho Variável) - OPCIONAL

- Agrega informações adicionais em relação à fragmentação, medição e monitoramento, controle e segurança, etc.


## Endereçamento

Composto de 32 bits

### Contagem binária

Base 2 → Seq. de bits 2ˆ3   2ˆ2   2ˆ1   2ˆ0
                  8        4      2      1

Ex: 101 = 5

- Utiliza-se blocos de 8 bits

- Varia de 0 a 255

- Antigamente estruturado em 5 classes (A, B, C, D, E)

- Hosts em uma mesma rede, NECESSARIAMENTE, possuem a mesma parcela de REDE


![[Pasted image 20250715151838.png]]


![[Pasted image 20250715151935.png]]


### Máscara de rede

32 bits em 4 blocos de 8 bits 

Define a identificação:

- Da REDE → Bit igual a 1
- Do HOST → Bit igual a 0



![[Pasted image 20250715152308.png]]

![[Pasted image 20250715152443.png]]


### Endereços reservados nas redes

Primeiro endereço → identificação da rede (todos os bits de HOST iguais a 0)

Último endereço → Utilizado para Broadcast (todos os bits de HOST iguais a 1)


![[Pasted image 20250715152808.png]]


<font color="#4bacc6">Obs:</font> Quantidade de Endereços EFETIVOS ou para HOSTS (<font color="#c0504d">TOTAL - 2</font>)


### Endereços reservados

- 0.0.0.0 → Utilizado na inicialização das máquinas

- 127.0.0.0 - Faixa para endereços de loopback (127.0.0.1)

- Permitem verificar o funcionamento de uma placa de rede

- Processados localmente e não são enviados pela rede


### Endereços Privados

Não são roteáveis na internet e, portanto, podem ser reutilizados

![[Pasted image 20250716114653.png]]





## Endereçamento (Subredes)

10 hosts em um ambiente

2 endereços reservados

Possibilidade de crescimento para 30 hosts

Pega-se bits emprestados de “HOST“ para se criar subredes

Sentido: <font color="#c0504d">Esquerda para Direita</font>

<font color="#4bacc6">ex:</font> 8 bits originais para subrede

3 bits emprestados → 2ˆ3 = 8 subredes

5 bits restantes para rede → 2ˆ5 = 32 endereços


## Fragmentação

Remontagem acontece <u>somente no destino</u>

Necessidade de controle e marcações dos fragmentos 

Definição do MTU da rede (Dados + Cabeçalho)

Ajuste do tamanho para que os dados possam ser trafegados 

Está presente na camada de rede


<font color="#c0504d">CAMPOS do CABEÇALHO : ID SEQ, FLAGS/MF E DF</font>
<font color="#c0504d">e FRAGMENT OFFSET</font>

<font color="#c0504d">CAMPO DE APOIO: Total Lenght</font>





