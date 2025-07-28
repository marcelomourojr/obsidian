# WPA

Baseado na especificação 802.11i, porém, não implementa todos os seus recursos

Utiliza <font color="#c0504d">RC4 atrelado ao TKIP</font> - Temporal Key Integrity Protocol

- IV de 48 bits

- Compatível com o WEP

## Versões:

- Personal - senha padrão

- Enterprise - sistema próprio de autenticação (802.1x/EAP)


## Funcionamento:

- PMK (primary master key) - Chaves de <u>32 a 512 bits</u>

- PTK (Pairwise Transient Key) - Chave gerada a partir de parâmetros da conexão (<u>512 bits</u>)
  -KCK (128 bits)
  -KEK (128 bits)
  -TEK (128 bits)
  -TMK (128 bits)

TKIP utiliza MIC - Message integrity Code (é como uma assinatura)