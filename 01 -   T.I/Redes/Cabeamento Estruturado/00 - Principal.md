
# Cabeamento Estruturado

#CabeamentoEstruturado #Redes #RedesDeComputadores 

## NBR 14565

- Possui como padrão a utilização de cabos UTP e conectores RJ-45

### [[000. Os 7 subsistemas|O sistema pode ser dividido em 7 tipos de subsistemas:]]

1. Cabeamento Horizontal (dentro)
2. Cabeamento de Backbase (dentro)
3. Sala de Telecomunicações
4. Sala de Equipamentos
5. Área de Trabalho
6. Entrada do Prédio
7. Interligação Externa (fora)

![[Pasted image 20250615160019.png]]

#### Cabeamento Horizontal

- Interconecta <u>a sala de telecomunicações às áreas de trabalho.</u>

- Geralmente faz a distribuição do cabeamento dentro de um <u>mesmo andar do prédio.</u>

- É composto por: Cabeamento Horizontal; Tomada de Telecomunicações; Terminações de Cabo e Cross-Connections.


#### Cabeamento de Backbone

- Interliga as <u>salas de telecomunicações às salas de equipamentos.</u>

- Contempla também a conexão da <u>Entrada do prédio à sala de Equipamentos.</u>


#### Sala de Equipamentos

- Armazena os principais equipamentos ativos de rede: servidores, switchs core, roteadores e PABX.


#### Sala de Telecomunicações

- Acomoda os equipamentos e terminadores de <u>distribuição.</u>

- Área de manobras do <u>cabeamento estruturado.</u>

- Interconecta <u>o cabeamento de backbone ao cabeamento horizontal através dos equipamentos da sala.</u>


#### Área de Trabalho

- Postos de trabalho (computadores, impressoras, telefones, etc)


#### Entrada do Prédio

- Interligação entre o cabeamento externo e o interno.

- <u>Ponto de chegada dos operadores</u> e outros serviços no edifício.

- <u>Geralmente fica dentro da sala de equipamentos.</u>


#### Interligação Externa

- Interligação entre prédios distintos, conectando a entrada do prédio A à sala de equipamentos do prédio B.


### Outras informações

- Topologia em Estrela

- Não possui mais de dois níveis hierárquicos de conectores de cruzamento (cross-connect)

- Os cabos que ligam os cross-connect não podem ultrapassar 20 metros.

- Evitar instalações em áreas onde existam interferências eletromagnéticas e rádio frequência.

- As instalações devem ser aterradas seguindo a norma EIA/TIA 607.


### Tipos de cabeamento

##### Cabo UTP de 100 Ohms (22 ou 24 AWG)
 - 800m para voz (20 a 300 MHz)
 - 90m para dados (Cat 3, 4 e 5)

##### Cabo STP (par trançado blindado) de 150 Ohms
- 90m para dados

##### Fibra óptica multimodo de 62,5 / 125 m 
- 2.000m para dados

##### Fibra óptica monomodo de 8,5 / 125 m
- 3.000m para dados


### Patch Panel

- Concentrador de cabos; Sistema passivo; Intermediário entre as tomadas de parede nas áreas de trabalho e outros pontos de conexão.

- Fornece um ponto de manobra do cabeamento horizontal em determinado ambiente.


### [[Regra 5-4-3]]

- 5 segmentos no total.

- 4 repetidores.

- 3 segmentos populados por máquina.

### Cabeamento de Datacenter

<font color="#9bbb59">EF:</font> Infraestrutura de entrada.

<font color="#9bbb59">ENI: </font>Interface de Rede Externa.

<font color="#9bbb59">BD:</font> Distribuidor de Edificio.

<font color="#9bbb59">FD: </font>Distribuidor de Piso.

<font color="#9bbb59">MD:</font> Distribuidor Principal.

<font color="#9bbb59">ZD:</font> Distribuidor de Zona.

<font color="#9bbb59">LDP:</font> Ponto de distruibuição Local.

<font color="#9bbb59">EO:</font> Tomada de Equipamento.
