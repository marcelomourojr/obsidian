## Spanning Tree protocol - 802.1d

STP - 802.1d

- Evitar loops na rede

- Criação de um único caminho operacional.

- Redes LAN são interligadas por diversos switches

- Estrutura hierárquica com redundância de links

- Evitar loops na rede




![[Pasted image 20250707110213.png]]



### Tipos de mensagens

<font color="#4bacc6">Hello Message</font> → “keep alive“ da root bridge a cada 2 seg

<font color="#4bacc6">Maximum Age Timer</font> → Tempo de validade de uma informação recebida via BPDU - 20 seg

<font color="#4bacc6">Forward Delay Timer</font> → Tempos limites de transição dos estados Listening & Learning - 15 seg

