
# ICMP

**Protocolo da camada de rede**

Fornece serviços de controle de tráfego e notificações de status

- Auxiliar ao IPv4

Fundamental para testes e troubleshooting :

- Testes de conectividade

- Mapeamento do encaminhamento de pacotes


## Estrutura

Tamanho de referência: 8 bytes

4 primeiros bytes fixos

Corpo da mensagem pode ser variável


## Principais mensagens 

**Echo Request** → Requisição para verificar se a máquina está ativa na rede

**Echo Reply** → Resposta a comando anterior, confirmando que a máquina está ativa

**Destination Unreachable** → Utilizado quando a rede ou o endereço de host de destino não pode ser alcançado ou encontrado

**Source Quench** →

**Redirect** →

**Time Exceeded** →

**Parameter Problem** →


![[Pasted image 20250722110127.png]]


## PING

Ferramenta de testes e Troubleshooting

Baseado nas mensagens ICMP:

- Echo Reply

- Echo Request

### Principais aplicações

Verificar o funcionamento da placa de rede através de um PING no endereço de loopback

Verificar o tempo de resposta entre os dispositivos


## TRACEROUTE / TRACERT

Traceroute → LINUX

Tracert → Windows

Traçar rota de pacotes, mapeando os nós;
Mapeamento de latência para identificar gargalos;
Identificar bloqueios

### Funcionamento

Manipula o campo TTL

Envia-se 3 pacotes UDP com TTL’s


