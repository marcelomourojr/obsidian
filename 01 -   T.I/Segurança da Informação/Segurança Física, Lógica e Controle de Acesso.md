
# Segurança Física, Lógica e Controle de Acesso


## Segurança Física

- Unidade de Alimentação Interruptiva (UPS)

- Gerador 

- Segurança Física

- Catracas

- SIte Físico Redundante 

- Travas de Equipamentos

- Alarmes

- Sala Cofre

- CFTV

## Segurança Lógica

Proteção dos recursos computacionais de todas as camadas desde a <font color="#c0504d">linguagem de máquina</font> e <font color="#c0504d">Kernel do SO,</font> passando pelo próprio sistema e todos os arquivos.

Pode-se utilizar firewalls, IDS, IPS, proxies, entre outros.


**HARDENING**: “endurecer“ um servidor, deixar ele mais robusto e seguro.


### Regras a serem seguidas:

<font color="#f79646">Acesso de ROOT</font>: Não se deve possibilitar a utilização do usuário ROOT de forma direta, logando-se como ROOT 

<font color="#f79646">Redução de Serviços: </font>Deve-se minimizar ao máximo o número de serviços rodando em um determinado servidor

<font color="#f79646">Limitação ao acesso remoto:</font> Configurar o servidor para o modo que apenas tenha acesso remoto com protocolos seguros como <font color="#c0504d">SSH</font>

<font color="#f79646">Atualização do Sistema</font>: é fundamental manter o sistema atualizado para reduzir falhas de segurança existentes 


## Controle de Acesso

### **Mandatory Access Control (MAC)**
O administrador é responsável por atribuir as permissões ao usuário

### **Discretionary Access Control (DAC)**
Mais flexível, o usuário tem o controle de garantir os privilégios de acesso a recursos que são de seu domínio. Ex: determinar as permissões do arquivo em que ele tem a posse

### **Role-Based Access Control (RBAC)**


