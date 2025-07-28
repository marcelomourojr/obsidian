
## Técnicas de detecção e correção de erros

### Verificação de paridade

- Método de certa forma ineficiente
- Utilização de bit de controle


### Checksum

- Muito utilizado na camada de transporte pelos protocolos TCP e UDP
- Baixo processamento 
- Utilizado quando se dá a nível de software


### Verificação de redundância cíclica - CRC

- Também conhecido como código polinomiais
- Esquema mais eficiente
- Exige grande processamento

* Ocorre a nível de hardware
* A quantidade de bits define o padrão - crc 8, crc 12, crc 16 ou crc 32
* Quanto maior a quantidade de bits, maior a capacidade de detecção


### Distância de Hamming

- Parâmetro que define a quantidade de bits que precisam ser corrigidos.

