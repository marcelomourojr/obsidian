
# Modelo Entidade-Relacionamento (MER)

#BancoDeDados #MER

Modelo conceitual para descrever as entidades (objetos), seus atributos (características) e como elas se relacionam (relacionamentos).

## Entidades (objetos)

### Física

Existente no mundo real como objetos físicos.
<font color="#9bbb59">Exemplos:</font> aluno, livro, automóvel…

### Lógica

Interação com entidade física, mas que no mundo real não são objetos físicos.
<font color="#9bbb59">Exemplos:</font> pedido, classificação…



# Diagrama Entidade-Relacionamento (DER)




<font color="#4f81bd">Entidades</font> (retângulos)                                                                                  <font color="#4f81bd">Relacionamento</font> (losango)

<font color="#c0504d">Atributos:</font> Acrescente mais camadas de detalhes ao adicionar atributos-chave de entidades. Atributos são frequentemente apresentados como ovais.



```mermaid
graph LR

    %% Atributos da entidade Pessoa
    Nome(("Nome")):::atributo
    Funcao(("Função")):::atributo

    %% Atributos da entidade Carro
    Placa(("Placa")):::atributo
    Modelo(("Modelo")):::atributo

    %% Entidades
    Pessoa["Pessoa"]:::entidade
    Carro["Carro"]:::entidade

    %% Relacionamento
    Lava{"Lava"}:::relacionamento

    %% Conexões retas com estilo DER tradicional
    Nome --- Pessoa
    Funcao --- Pessoa
    Pessoa --- Lava
    Lava --- Carro
    Carro --- Placa
    Carro --- Modelo

    %% Estilos personalizados
    classDef entidade fill:#ffffff,stroke:#000000,stroke-width:2px;
    classDef atributo fill:#ffffff,stroke:#000000,stroke-width:1px;
    classDef relacionamento fill:#ffffff,stroke:#000000,stroke-width:2px;