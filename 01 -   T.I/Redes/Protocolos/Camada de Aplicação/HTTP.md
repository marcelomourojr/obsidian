
# HTTP (Hypertext Transfer Protocol)

Cliente - Servidor no modelo Requisição / Resposta

Porta 80, Codificação ASCII

Protocolo Stateless

## URI (Identificador Universal de Recurso)

Une o Protocolo, a URL e o nome do recurso (URN)

## URL ( Uniform Resource Locator) 

Se refere ao local, o host que você quer acessar determinado recurso

## URN (Uniform Resource Name)

Nome do recurso que será acessado e também faz parte da URI (Como: home.html, contato.php)


## Métodos HTTP:

**GET**: solicita dados de um recurso.

**POST**: envia dados para serem processados (ex: formulário).

**PUT**: substitui completamente um recurso.

**DELETE**: remove um recurso.

**PATCH**: atualiza parcialmente um recurso.

**HEAD**: solicita apenas os cabeçalhos de resposta, sem o corpo.

**OPTIONS**: retorna os métodos suportados por um servidor.

**TRACE**: método menos comum, usado para depuração, retorna a requisição recebida pelo servidor, útil para verificar o caminho que a requisição percorreu.

### Classificação dos Métodos

Idempotente → Get, Put, Head, Delete.

Não idempotente → Post


## Códigos de Estado

1XX → <font color="#c0504d">Classe Informacional</font>

2XX → <font color="#c0504d">Classe de Sucesso</font>

3XX → <font color="#c0504d">Classe de Redirecionamento</font>

4XX → <font color="#c0504d">Classe de Erros do Cliente</font>

- 400 (Bad Request) → Erro de sintaxe
- 401 (Unauthorized) → Depende de autenticação do usuário
- 403 (Forbidden) → O servidor recusa a atender a requisição
- 404 (Not Found) → Não encontrou o endereço

5XX → **Classe de Erro do Servidor**

- 500 → Erro inesperado
- 503 → Sobrecarga ou manutenção, Condição temporária
- 505 → Versão não suportada


## Cache Web

Tenta viabilizar uma resposta rápida para consultas idênticas 

Formas: Servidor PROXY, PROXY Reverso e Cache local

### Servidor PROXY

- Elemento intermediário entre o cliente e servidor

- Todas as consultas passam pelo PROXY em uma rede interna (duas conexões)

### PROXY reverso

- Proteção aos servidores de destino

- Possibilita o balanceamento de carga

- Armazenamento em CACHE das informações estáticas

### CACHE local

- Browsers armazenam informações recebidas do servidor




## Versões

**HTTPv1.0** → Não realiza conexões persistentes. Para cada mensagem, abre-se uma nova conexão.

**HTTPv1.1** → Realiza conexões persistentes. Em uma mesma conexão TCP, envia-se várias mensagens.

**HTTPv2.0** → Aumentou o desempenho, com uma quantidade maior de conexões. Contemplar dinâmica de responsabilidade para navegação em dispositivos móveis com baixo consumo e maior desempenho

- Compressão automática

- Criptografia e Segurança


**HTTPv3.0** → Utiliza o QUIC ao invés do TCP

- Multiplexado de transporte sobre o UDP

- Implementa detecção de perda e retransmissão separadamente para cada fluxo (stream). Isola os processos de recuperação




