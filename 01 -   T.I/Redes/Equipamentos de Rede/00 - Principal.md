
# Equipamentos de Rede

#EquipamentosDeRede #Redes 

## MODELO OSI

### Dividida em 7 camadas:

1. Física

2. Enlace

3. Redes

4. Transporte

5. Sessão

6. Apresentação

7. Aplicação



### Domínios de Colisão

- Concorrência no meio para transmissão.

- Todos recebem a informação transmitida no meio

- Somente uma transmissão por vez.

- Visibilidade <font color="#c0504d">até a segunda camada do modelo OSI (Enlace)</font>

- Banda disponível compartilhada por todos e limitada ao de menor velocidade.


### Domínios de Broadcast

- Domínio lógico que <u>identifica os dispositivos dentro de uma mesma rede.</u>

- Só serão transmitidos a todos se houver um comando para isso.

- Representa o isolamento lógico entre redes.

- É formado por um agrupamento de domínios de colisão.

- Visibilidade <font color="#c0504d">até a terceira camada do modelo OSI (Rede)</font>



## Os principais elementos são:

1. [[01 -   T.I/Redes/Equipamentos de Rede/00 - Principal#Placas de Rede|Placas de Rede]]

2. Repetidor

3. Concentradores ou HUBs

4. Bridges

5. Switchs

6. Roteadores

7. Gateways

8. Access Points


### Placas de Rede

- Permitem a comunicação dos equipamentos entre si através da rede.

- Cada placa possui um endereço físico único chamado MAC (formado por 48 bits e escrito no formato hexadecimal)



### Repetidores Hubs ou Concentradores

- Atua na <font color="#c0504d">camada 1 (Física)</font> do modelo OSI

- Interconecta segmentos de rede
    -Mesmo domínio de colisão
    -Mesmo domínio de Broadcast

- Comunicação Half Duplex

- Dados propagados em todas as pontas

- Evolução do Repetidor

#### TIPOS

<font color="#c3d69b">Ativos</font>
- Restaura a amplitude do sinal, forma e sincronismo; Depende de energia.

<font color="#c3d69b">Passivos</font>
- Simplesmente replica o sinal recebido.

<font color="#c3d69b">Inteligentes</font>
- Gerência mínima da rede.



#### TOPOLOGIAS

Topologia Física: <font color="#c0504d">ESTRELA</font> 

Topologia Lógica: <font color="#c0504d">BARRAMENTO</font>


### Repetidores

- Busca estender o alcance de uma rede.

- Possui apenas duas portas

- Possui o recurso de regenerar o sinal, bem como o hub ativo.




### Bridges 

- Atuam na <font color="#c0504d">camada 2 (enlace)</font> do modelo OSI.

- Possuem apenas 2 portas.

- <font color="#c0504d">Isolam os domínios de colisão entre suas interfaces.</font>
 O tráfego só passará para a outra porta caso seja necessário, ou seja, o destinatário esteja no outro segmento

- <font color="#c0504d">Um único domínio de broadcast.</font>

- Tem uma tabela interna para mapear os dispositivos (Endereço MAC)


![[Pasted image 20250617214307.png]]


### Switches

- Atuam na <font color="#c0504d">camada 2 (enlace)</font> de forma nativa.

- Várias portas

- <font color="#c0504d">Isolam os domínios de colisão entre suas interfaces.</font>

- <font color="#c0504d">Um único domínio de broadcast (sem utilizar VLAN).</font>

- Também utiliza tabela para mapear os dispositivos (endereço MAC).
   -Tabela CAM (Content Addressable Memory) de tamanho limitado.

- 3 tipos de tráfego - Unicast, Broadcast e Multicast.

- Existem switches que atuam até <font color="#c0504d">a camada 7 do modelo OSI.</font>

- Os mais utilizados são os de camada 3 ou switches L3.
  -Usa endereços de rede para encaminhar pacotes, implementando técnicas de roteamento.
  -<u>Capaz de segmentar domínios de Broadcast.</u>

- Capacidade de rotear pacotes a nível de hardware, diferente dos <font color="#c0504d">roteadores</font> <u>que atuam a nível de software.</u>


![[Pasted image 20250617214710.png]]


### Roteadores

- São nativos da <font color="#c0504d">camada 3 (Rede)</font> do modelo OSI

- Utiliza <font color="#c0504d">endereços IP ou de rede.</font>
   -Tabelas de roteamento
   -<u>Algoritmo a nível de software</u>

- Processamentos a <u>nível de software.</u>

- <u>Capaz de isolar domínios de Colisão e Broadcast entre suas interfaces.</u>

- Possuem quantidades de portas menor quando comparado aos switches:
  -Roteadores: 2,4 ou 8;
  -Switches: 24,48 ou 96;

- Capacidade de interconectar segmentos com <u>tecnologias diferentes</u> a nível da tomada de <u>enlace</u>.


### Gateways

#### Diferentes conceitos do termo Gateways:

- Gateway como escoamento de tráfego em uma rede.

- Gateway como elemento de conexão.

- Atuam em todas as camadas do modelo OSI.
  -É um equipamento da camada 7.

- Utilizado para comunicação de diferentes <u>protocolos e tecnologias.</u>


<font color="#c3d69b">Criado para cada aplicação com tecnologias diferentes:</font>

- Gateways de voz (TDM para IP)

- Gateways de rede (IP e IPX)


### Encapsulamento - Modelo OSI

![[Pasted image 20250618204736.png]]

![[Pasted image 20250618204813.png]]


### Camada 1 (Física) - Modelo OSI

<font color="#9bbb59">Simplex </font>- Unidirecional

<font color="#9bbb59">Half Duplex</font> - Bidirecional de forma não simultanea

<font color="#9bbb59">Full Duplex</font> - Bidirecional de forma simultanea


**Responsável pela conversão da sequência de bits em sinais elétricos.**


### Camada 2 (Enlace) - Modelo OSI

<u>Receber a informação em uma interface e repassá-la a uma ou várias portas do mesmo tipo.</u>

#### Tipos

1. Comutação por Circuitos
2. Comutação por Pacotes
3. Comutação por Mensagens


#### Subdivisão da camada Enlace

- MAC (Media Access Control)
- LLC (Logical Link Control)

##### MAC

- Subcamada inferior

- Fornece os meios necessários para <u>o efetivo acesso ao meio.</u>

- Implementa as <u>tecnologias de acesso ao meio.</u>

- <u>CSMA/CD</u> ou <u>CSMA/CA.</u>

##### LLC

- Subcamada inferior.

- Realiza a <u>checagem e a correção dos quadros.</u>

- Responsável pela sincronia dos <u>pacotes recebidos</u> da camada superior.

- Mantém as <u>relações lógicas entre os dispositivos.</u>


### Camada 3 (Rede) - Modelo OSI

- Implementa a <u><font color="#c0504d">fragmentação e remontagem dos pacotes</font></u>

- Depende da <u>capacidade de transmissão do meio</u>, conhecido como <u>MTU</u> (Max Transfer Unit) padrão 1500
  -Define a quantidade de bytes que o enlace suporta
  -Desconsidera o cabeçalho da camada de enlace

- Implementa técnicas de controle de erro.

**Provê uma comunicação Nó-a-Nó ou Ponto-a-Ponto.**


### Camada 4 (Transporte) - Modelo OSI

Realiza a <font color="#c0504d"><u>Segmentação</u></font> dos dados recebidos da camada superior.


<font color="#c0504d">Pode implementar diversas</font> técnicas:
- controle de fluxo.
- ordenação de pacotes.
- detecção e correção de erros.
- detecção de perda e duplicação de pacotes FIM-A-FIM.


Utiliza o conceito <u>MSS (Max Segment Size)</u>
- Baliza o valor de referência de acordo com as informações do MTU

### Camada 5 (Sessão) - Modelo OSI

- Implementa recurso de <u>estabelecimento e suporte</u> de sessões dos serviços das camadas superiores.

- Correlaciona os <u>processos</u> em execução nos dispositivos de origem e destino.

- Utiliza marcação nos dados que permitem o retorno à comunicação a partir da sessão previamente estabelecida.


### Camada 6 (Apresentação) - Modelo OSI

- Responsável <font color="#c0504d">pela formatação dos dados</font> a serem transmitidos e recebidos em um formato comum e compreensível.

- Pode implementar técnicas <font color="#c0504d">de compressão e criptografia dos dados:</font>
  -Compressão busca aumentar a eficiência.
  -Criptografia busca agregar mais segurança.


### Camada 7 (Aplicação) - Modelo OSI

- Camada mais próxima do usuário final

 - Recursos implementados a nível de software.

- Permite a comunicação dos processos das aplicações e usuários com os serviços de rede.

