
# Topologias de Redes

#Redes #TopologiasDeRedes

### Fatores importantes

- Confiabilidade, Disponibilidade e Redundância.

- Velocidade de Transmissão.

- Custo de Manutenção.

- Escalabilidade.


<font color="#c0504d">Esses fatores definem qual topologia será a mais recomendada para determinado ambiente frente aos requisitos apresentados.</font>



## Principais Topologias

- Barramento

- Anel

- Estrela

- Mesh e Full Mesh

- Árvore ou Hierarquizada


### Barramento (BUS)

- Utiliza o método de <font color="#c0504d">difusão (broadcast)</font> em uma conexão multiponto.

- Pode utilizar forma de <font color="#c0504d">controle de acesso ao meio físico</font> centralizado ou descentralizado para evitar colisões das informações trafegadas.

- Escalável até o limite suportado pelo barramento.

- <font color="#c0504d">Não é seguro</font>, pois a informação está disponível a todos no meio.

- Excelente <font color="#c3d69b">tolerância a falhas</font>.


### Anel 

- Conexões <font color="#c0504d">ponto-a-ponto</font>.

- Dependência de nós intermediários .

- À medida que cresce, a comunicação pode ficar lenta, não sendo escalável.

- <font color="#c0504d">Não é seguro</font>, pois a informação estará disponível a todos no meio.

- <font color="#c0504d">Altamente susceptível a falhas</font>. 

- Utiliza tokens para determinar o acesso ao meio.

- NATIVO: <font color="#c0504d">anel unidirecional</font>.

- SEM SER NATIVO: Pode ter tráfego <font color="#c0504d">bidirecional</font>; Para aumentar a confiabilidade e disponibilidade, utiliza um anel secundário; 


### Estrela

- Conexões <font color="#c0504d">ponto-a-ponto</font> em torno de um <font color="#c0504d">nó central</font> que comutará as mensagens.

- Necessita de controle de acesso ao meio.

- Boa tolerância a falhas, apesar de <font color="#c0504d">existir um ponto crítico de falha</font>.

- Expansão e processamento depende do <font color="#c0504d">nó central</font>.


### Mesh ou Malha

- Interconexão ponto-a-ponto entre <font color="#c0504d">ALGUNS nós</font>.

- <font color="#c0504d">Pouco escalável</font>.

- <font color="#c3d69b">Excelente tolerância a falhas</font>.

- Desempenho vinculado aos <font color="#c0504d">enlaces entre cada par</font>.

- Existe a rede <font color="#4bacc6">FULL MESH</font> (<font color="#b7dde8">Conexão entre TODOS os dispositivos</font>).


### Árvore

- Hierarquização

- Deriva da rede estrela.

- Topologia utilizada na maioria dos ambientes de rede.

- Possui <font color="#c3d69b">boa escalabilidade</font> e <font color="#c3d69b">tolerância a falhas</font>.



## Topologia Lógica X Física

### Definição

##### TOPOLOGIA LÓGICA
Forma como os dados são trafegados.
##### TOPOLOGIA FÍSICA
Forma como os nós são interconectados.

- Topologia Lógica opera sobre a topologia Física.


## CSMA/CD x CSMA/CA

### CSMA/CD (Carrier Sense Multiple Access with Collision Detection)

#### Etapas:

1. O nó verifica se o meio está livre para transmissão.

2. Estando livre, o nó começa sua transmissão mantendo a escuta do meio com a tecnologia LWT <font color="#c0504d">(Listen While Talk)</font>

3. Caso identifique um outro sinal sendo transmitido, inicia-se o algoritmo de recuperação <font color="#c0504d">(backoff)</font> para estabilização do meio e futura retransmissão: Envia-se um sinal JAM divulgando a colisão; Todos param de transmitir imediatamente; Os que desejam transmitir, aguardam um tempo aleatório.


### CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance)

#### Etapas:

1. O nó verifica se o meio está livre para transmissão.

2. Estando livre, o nó envia um pacote informacional a todos os dispositivos dizendo o tempo que pretende ocupar o meio para transmitir os dados.

3. As demais estações tomam ciência e nem mesmo verificam o meio durante esse período.


