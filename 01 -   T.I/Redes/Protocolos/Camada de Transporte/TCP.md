
# TCP - (Transmission Control Protocol)

- Confiável

- Orientado à conexão - (3-way-handshake)

- Verificação de erros fim a fim 

- Recuperação de Perda de Pacote e descarte de pacotes duplicados

- Controle de Fluxo


## Cabeçalho

**<font color="#c0504d">Possui 20 bytes de cabeçalho</font>**

**Source Port (16 bits)** → Porta de origem

**Destination Port (16 bits)** → Porta de destino

**SEQ Number (32 bits)** → Número de sequência para controle de recebimento e confiabilidade

**ACK Number (32 bits)** → Número de sequência esperados

**Data Offset** → Tamanho de cabeçalho para demarcação do início dos dados

**URG** → Gera interrupções para ter prioridade

**ACK** → Se ativado, lê o ACK Number

**PSH** → Envio direto à camada superior sem armazenar em buffer

**RST** → Reinicia a conexão

**SYN** → Estabelecimento de conexão

**FIN** → Encerramento de conexão

**Window (16 bits)** → Controle de fluxo

**Checksum (16 bits)** → Detecta erros <font color="#c0504d">em todo o segmento</font>


## Estabelecimento da Conexão

**3-Way-Handshake** → Necessariamente deve ocorrer a troca das 3 mensagens de sinalização para estabelecimento da conexão


## Encerramento da Conexão

<font color="#c0504d">Pode ocorrer em 4 ou 3 vias</font>

- 3-way handshaking e fourway handshaking 


## Segmentação

**MMS - Maximum Segment Size**

- Realiza a segmentação dos dados da camada superior

- Ocorre fim a fim


