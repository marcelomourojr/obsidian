# WEP

Algoritmo utilizado: <font color="#c0504d"><u>RC4</u></font>

Aplica o conceito de <font color="#c0504d">Vetor de Inicialização - IV de <u>24 bits</font></u>

Chave de <font color="#c0504d"><u>40 bits</u></font> ou <font color="#c0504d"><u>5 bytes (senha-padrão)</u></font>

Há implementações com chaves total de 128 bits ou 16 bytes, ainda que o RC4 suporte 2048 bits ou 256 bytes.

Utiliza o <u>CRC32</u> para garantia da integridade.

## Funcionalidades 

### KSA (Key Scheduler Algorithm)

- Gera a chave

### PRGA (Pseudo Random Generation Algorithm)

- Encripta a mensagem a partir do resultado do KSA

## 2 fases : Autenticação e Encriptação


## Vulnerabilidades:

- Ataques de Força Bruta dada a chave pequena 

- Reutilização do vetor de inicialização

- Possibilidade de manipulação do CRC32

- Softwares de quebra: airSnort e WepCrack




![[Pasted image 20250711100616.png]]

