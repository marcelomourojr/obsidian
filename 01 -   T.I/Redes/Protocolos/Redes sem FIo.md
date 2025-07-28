
## Redes sem fio

WLAN → 802.11

### 802.11z 

**Otimização da comunicação**

- Utiliza a tecnologia <u>TDLS</u> (Tunneled Direct Link Setup)

- Cria um túnel direto entre os dispositivos, <u>sem depender do Access Point</u>.

- Diferente do WIFI DIRECT, que visa apenas o estabelecimento rápido da conexão.


### FHSS - Frequency Hope Spread Spectrum

- 79 Subfaixas de 1 MHz a partir da frequência 2.4 MHz.

- Distribuição aleatória nas faixas de frequência durante a transmissão.


### DSSS - Direct Sequence Spread Spectrum

- 14 canais de 22 MHz a partir da frequência 2.4 MHz

- Distribuição sequencial nas faixas de frequência durante a transmissão.

- Disponibiliza apenas 3 canais sem sobreposição: 1, 6 e 11.


### OFDM - Ortogonal Frequency Divison Multiplexing

- Aplica o conceito de ortogonalidade de subportadoras em frequência para aumentar a eficiência de uso da banda de transmissão.


### MIMO - Multiple IN, Multiple OUT

- A partir do 802.11n

- Baseado no conceito de fluxos distintos por caminhos diferentes.

- Utilizam-se várias antenas para originar e recolher o sinal de forma simultânea.

#### Estrutura - n x m : s

N - Antenas de Transmissão

M - Antenas de Recepção

S - Fluxos de dados

Limite: 4 x 4 : 4


### 802.11e

- Conjunto de aprimoramentos de QoS na subcamada MAC da camada de enlace

- Prioriza o tráfego de maior prioridade, permitindo a propagação de diferentes classes de tráfego - EDCA

### Modos de operação - 802.11

- DCF - Distributed Coordination Function

- PCF - Point Coordination Function

#### DCF

- Independe de um controle central

- <u>Utiliza o CSMA/CA</u>

##### Formas de atuação

- Meio disponível, envia-se o sinal, sem a capacidade de escutar o meio.

- Aspectos de sinalização e confirmação. Minimiza o problema do terminal escondido.

### PCF

- Nó central controla a alocação do meio.

- Processo de “POLLING“

### DCF e PCF

- Possiblidade de atuarem juntos

- Definição de intervalos obrigatórios

#### SIFS (Short InterFrame Spacing)

<u>Após esse intervalo</u>, somente fragmentos de pacotes que já estejam <u>sendo transmitidos</u> ou <u>ACK’s
</u>
#### PIFS (PCF InterFrame Spacing)

Após esse intervalo, o nó central pode realizar o processo de POLLING

#### DIFS (DCF InterFrame Spacing)

Após esse intervalo, <u>qualquer nó</u> pode ocupar o meio. Alta probabilidade de colisão.


#### EIFS (Extended InterFrame Spacing)

Após esse intervalo, estações que receberam pacotes <u>corrompidos</u> ou <u>defeituosos</u> podem informar. <u>Menor Prioridade</u>


### 802.15

- WPAN

#### Subgrupos:

TG4 Low Rate: baixas taxas (20 Kbps a 250 Kbps)

TG3 High Rate: altas taxas (11 Mbps a 55 Mbps)

### 802.15.1 - Bluetooth

- Opera na faixa de 2.4 GHz e utiliza TDM

- Redes AD HOC

- Baixo custo, pouco alcance, baixa potência e baixa taxa de transferência (até 4 Mbps)

- Dispositivos organizados em pequenas redes (piconet)

- Elege-se um master (mestre) e os demais são chamados de Slave (escravos)

- Até 7 nós ativos escravos por piconet

- Até 255 em modo estacionado

Modos

HOLD (Para nós de interconexão)

SNIFF (Período específico para ativo-inativo)

PARK (Passa-se para inatividade)

### 802.15.4 Bluetooth - Zigbree

- Rede confiável, baixa potência, baixa taxa de transmissão e é a principal aplicação para automação residencial.

### 802.16 - Wimax

- Em redes WMAN

- Faixas de frequência mais elevadas (10 GHz a 66 GHz)

- Redes de infraestrutura (Ponto de Acesso ou estação-rádio base)

#### Subpadrões:

802.16d - Técnica MIMO

802.16e - Modalidade com velocidade acima de 100 Km/h





![[Pasted image 20250708104607.png]]



![[Pasted image 20250708223130.png]]