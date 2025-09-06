
![[Pasted image 20250905153029.png]]

## Protocolos da camada de enlace

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


#### Cabeçalho 802.3

**Preâmbulo** → Utilizado para sincronia e sequenciamento.
- 7 bytes com bits alternados
- 1 byte chamado de SFD (Start Frame Delimiter)

![[Pasted image 20250625122709.png]]


**O cabeçalho possui 18 bytes**

![[Pasted image 20250625122759.png]]


#### Modos de Operação (Comutação)

##### 4 modos de operação

- [[01 -   T.I/Redes/Protocolos/00 - Principal#Store-and-forwand| Store-and-forwand]]

- [[01 -   T.I/Redes/Protocolos/00 - Principal#Cut-through ou Fast Forward| Cut-through ou Fast Forward]]

- [[01 -   T.I/Redes/Protocolos/00 - Principal#Fragment Free| Fragment Free]]

- [[01 -   T.I/Redes/Protocolos/00 - Principal#Adaptative Cut Through|Adaptative Cut Through]]



###### Store-and-forwand

- Armazena (buffers) e Encaminha

- Método mais lento e com maior latência

- Deve-se ler o quadro completo

- Caso não possua tamanho mínimo e máximo suficiente, <u>descarta-se o quadro.</u>


###### Cut-through ou Fast Forward

- Lê apenas os <u>6 primeiros bytes</u> e encaminha.

- Menor latência

- Maior chance de erros e com menor confiabilidade.
  -Não verifica erros
  -Não verifica se o quadro está corrompido


###### Fragment Free

- Leitura dos 64 primeiros bytes

- Latência média com boa filtragem de erros

- Verifica a intregridade de tamanho mínimo


###### Adaptative Cut Through

- Método inteligente que faz uso dos demais métodos

- Configurável de forma manual ou automática

- Pode mudar de um estado para <span class="underline-red">outro durante a operação.</span>




#### Modelo Hierárquico

- Diz respeito a como são arranjados os diversos switches em uma rede complexa.

- Dividido em até 3 camadas
  -Pode operar com 2 ou até 1

##### Acesso

- Camada mais próxima dos usuários ou dos dispositivos.

- Implementação de <u>controles de acesso</u>:
  -Autenticação <u>802.1x</u>
  -<u>Marcação de Vlan’s</u>


##### Distribuição

- Agregação de Vlan’s → Trunk

- Provê a comunicação entre os switches de acesso.

- Algumas políticas de <u>controle de tráfego</u> → como ACL.


##### Core 

- Concentrará o tráfego das camadas inferiores.

- Conhecido como BackBone de <u>alta velocidade e redundância</u>.

- Principais dispositivos em uma rede complexa.

- Maior investimento em uma rede.



#### Técnicas de detecção e correção de erros

##### Verificação de paridade

- Método de certa forma ineficiente
- Utilização de bit de controle


##### Checksum

- Muito utilizado na camada de transporte pelos protocolos TCP e UDP
- Baixo processamento 
- Utilizado quando se dá a nível de software


##### Verificação de redundância cíclica - CRC

- Também conhecido como código polinomiais
- Esquema mais eficiente
- Exige grande processamento

* Ocorre a nível de hardware
* A quantidade de bits define o padrão - crc 8, crc 12, crc 16 ou crc 32
* Quanto maior a quantidade de bits, maior a capacidade de detecção








