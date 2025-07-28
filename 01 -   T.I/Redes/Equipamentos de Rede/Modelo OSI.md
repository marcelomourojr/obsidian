
## MODELO OSI

### Dividida em 7 camadas:

1. Física

2. Enlace

3. Redes

4. Transporte

5. Sessão

6. Apresentação

7. Aplicação


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