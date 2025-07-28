
# IGMP

Atua na camada de rede

Somente IPv4

Utiliza as faixas de endereço da classe D

Define como as mensagens serão trocadas entre os roteadores para atualização das listas de multicast

Responsável por gerenciar a entrada e saída dos hosts no grupo

Responsável por gerenciar grupos de multicast


## Estados:

<font color="#4bacc6">Non - Member</font> → Quando o host não pertence ao grupo

<font color="#4bacc6">Delaying - Member</font> → Quando o host pertence e possui um temporizador para relatórios em execução

<font color="#4bacc6">Idle - Member</font> → Quando o host pertence ao grupo e não possui o temporizador



## Estrutura:

<font color="#4bacc6">Version</font> → Versão do protocolo (1, 2 ou 3)

<font color="#4bacc6">Checksum</font> → Integridade do pacote

<font color="#4bacc6">Type</font> → Tipos de mensagens: 

- <font color="#fbd5b5">Host Membership Report</font> → Enviada pelo <u>host</u> no momento de sua associação ao grupo Multicast.

- <font color="#fbd5b5">Host Membership Query</font> → Enviada pelo <u>roteador</u> com vistas a pesquisar membros nos grupos Multicast.

- <font color="#fbd5b5">Group Leave</font> → Enviada por aqueles hosts que não desejam mais receber o tráfego de determinado grupo Multicast. <u>Esta mensagem é opcional</u>.

