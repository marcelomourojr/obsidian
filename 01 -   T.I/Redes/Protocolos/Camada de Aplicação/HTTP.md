
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

## Versões

**HTTPv1.0** → Não realiza conexões persistentes. Para cada mensagem, abre-se uma nova conexão.

**HTTPv1.1** → Realiza conexões persistentes. Em uma mesma conexão TCP, envia-se várias mensagens.

**HTTPv2.0** → Aumentou o desempenho, com uma quantidade maior de conexões. Contemplar dinâmica de responsabilidade para navegação em dispositivos móveis com baixo consumo e maior desempenho

- Compressão automática

- Criptografia e Segurança


**HTTPv3.0** → Utiliza o QUIC ao invés do TCP

- Multiplexado de transporte sobre o UDP

- Implementa detecção de perda e retransmissão separadamente para cada fluxo (stream). Isola os processos de recuperação




