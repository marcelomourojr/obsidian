# Modelo ATM

Possui protocolos


- Comutação por células.

- Tamanhos fixos de 53 byes
  -5 bytes de cabeçalho e 48 bytes de conteúdo

- Orientado à conexões.

- Independente de sincronia entre relógios de origem e destino.

- Atua tanto em redes LAN quanto em WAN

- Comutação a nível de hardware


![[Pasted image 20250630104424.png]]




![[Pasted image 20250630104532.png]]


## AAL (ATM Adaption Layer)

- Faz-se a conversão e segmentação em células ATM e vice-versa.

- Controla erros de transmissão.

- Controla o fluxo entre os protocolos superiores.

### Subdividida em:

#### CS (Convergence sublayer)

- Permite que o ATM forneça serviços a diversos protocolos, serviços e aplicações.

#### SAR (Segmentation and reassembly)

- Divide os pacotes em células na origem e reagrupa no destino.


## ATM Layer

- Transporte de células

- Controle dos <u>circuitos virtuais</u> e <u>controle de congestionamento</u>.


## Physical Layer

- Semelhante a camada física do modelo OSI

- Sinais elétricos ou ópticos, sincronização de bits, entre outros.

### Subdividida em:

#### TC (Transmission convergence)

- Faz a conversão das células em sequência de bits.

#### PMD (physical medium dependent)

- Conexão entre a interface e o meio. Controle de sincronismo.




![[Pasted image 20250630121435.png]]


## Classes de serviços

### <font color="#1f497d">CBR - Constant</font> bit rate ou classe A

- Utilizado em conexões com banda fixa e taxa constante

### <font color="#1f497d">VRB - Variable</font> bit rate ou classe B

- Pode ser em tempo real ou não.
- RT-VRB variação mínima na taxa.

### <font color="#1f497d">ABR - Available</font> bit rate ou classe C

- Depende da disponibilidade; Transferencia em rajadas quando há disponibilidade.

### <font color="#1f497d">UBR - Unspecified</font> bit rate ou classe D

- Classe mais volátil e que menos fornece recursos e qualidade às aplicações. Possui menos critério de qualidade de serviço.


### AAL 0 

- Não implementa tratamento diferenciado de tráfego. Também conhecido como “RAW CELL“. Mantém a área útil de dados em 48 bytes.

### AAL 1

- Suporta <u>CBR</u> com tráfego sincronizado. Utiliza <u>um bit de área útil de dados </u>para implementação. Utilizado para tráfego de voz <u>sem</u> compressão.

### AAL 2

- Suporta <u>VBR</u> com tráfego sincronizado. Utiliza um bit de área útil de dados para implementação. Utilizado para tráfego de voz <u>com</u> compressão

### AAL 3/4

- Suporta ABR com tráfego Assíncrono. Utiliza 4 bytes da área útil de dados para sua implementação.


### AAL 5

- Similar ao AAL 3/4; Implementação mais simplificada; Utilização do UBR; Formato mais utilizado.


## Modelo tridimensional


### 1 - Plano de usuário

- Controle de fluxo, correção de erros, transporte de dado e outras funções de usuários.

### 2 - Plano de controle

- Gerenciamento de conexões.

### 3 - Plano de gerenciamento 

- Coordenação e interação entre camadas e gerenciamento de recursos.





