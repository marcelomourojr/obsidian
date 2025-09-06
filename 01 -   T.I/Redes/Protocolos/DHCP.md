
# DHCP

Comunicação com o Servidor DHCP  

O cliente DHCP utiliza a porta UDP **68 p/ enviar solicitações** de DHCP ao servidor DHCP.

O servidor DHCP utiliza a **porta UDP 67 para receber solicitações** dos clientes DHCP e enviar as respostas contendo as configurações de rede apropriadas.

**DORA**

<font color="#f79646">DHCP DISCOVER</font> – enviado pelo cliente, para  
identificar servidor DHCP na rede.

<font color="#f79646">DHCP OFFE</font> – enviado pelo servidor ao cliente  
para ofertar o endereço de IP.

<font color="#f79646">DHCP REQUEST</font> – enviado pelo cliente ao servidor  
aceitando a oferta.

<font color="#f79646">DHCP ACK</font>– evento enviado do servidor para o cliente  
aceitando a comunicação.


<font color="#9bbb59">DHCP relay</font> é um roteador ou host que propaga as solicitações de um cliente a um servidor que está em outra rede e vice-versa.