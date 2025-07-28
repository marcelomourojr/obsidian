### Ethernet

- Taxas de 10 Mbps em modo Half-Duplex.

- Foi baseado em redes com HUB.

- Quadros com tamanhos de 1500 bytes.

- Utiliza o método [[Manchester]].

- Tecnologias:
  -10baseT → Par trançado.
  -10base2 → Cabo coaxial fino (THINNET).
  -10base5 → Cabo coaxial grosso (THICKNET).


#### Endereço MAC

Formato hexadecimal e formado por 48 bits.

- Unicast → 1 para 1 → par x4-xx-xx-xx-xx-xx

- Multicast → 1 para muitos → ímpar x9-xx-xx-xx-xx-xx

- Broadcast → 1 para todos → FF-FF-FF-FF-FF-FF


### FastEthernet

- Principal padrão utilizado em redes LAN (agora também Gigabit Ethernet).

- Taxas de 100 Mbps suportando FULL-Duplex.

- Codificação 4B/5B.

- Tecnologias:
  -100Base TX → Utilizada dois dos quatro pares disponíveis.
  -100Base SX → 
  -100Base LX →


### GigaBitEthernet

- Taxas de 1000 Mbps ou 1 Gbps.

- Apenas modo FULL-DUPLEX.

- Codificação 8B/10B.

- Depende minimamente de cabeamento CAT 5 (4 pares)
  -Recomenda-se uso de CAT 5e ou 6 (2 pares)

- Método Flowcontrol.

- Suporte ao <u>Jumbo Frame (9.000 bytes)</u>

- Suporte ao FrameBurst.

- Depende de switch L2.

- Não suporta utilização de hubs ou bridges.

- Não utilizam CSMA/CD.

- Cabeamento mínimo de par trançado, Cat 6. (Cat 6a é o recomendado).

- Exemplos de tecnologia:
  -1000baseTX
  -1000baseSX
  -1000baseLX
  -1000baseCX


### Cabeçalho 802.3

**Preâmbulo** → Utilizado para sincronia e sequenciamento.
- 7 bytes com bits alternados
- 1 byte chamado de SFD (Start Frame Delimiter)

![[Pasted image 20250625122709.png]]


**O cabeçalho possui 18 bytes**

![[Pasted image 20250625122759.png]]


