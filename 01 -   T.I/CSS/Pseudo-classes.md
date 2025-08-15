selector:pseudo-class -> Usada para definir um estado especial de um elemento.

Pseudo Classes

:active                             a:active                           Seleciona o link ativo

:hover                              a:hover                          Seleciona links ao passar o mouse

:link                                  a:link                              Seleciona todos os links não visitados

:visited                            a:visited                          Seleciona todos os links visitados

:checked                          input:checked             Seleciona cada elemento <input> marcado

:disabled                          input:disabled           Seleciona cada elemento <input> desabilitado

:empty                              p:empty                     Seleciona cada elemento que não tem filhos

:enabled                           input:enabled            Seleciona cada elemento <input> habilitado

:first-child                          p:first-child               Seleciona todos os elementos <p> que são o primeiro filho de seu pai

:first-of-type                     p:first-of-type        Seleciona cada elemento <p> que é o primeiro elemento <p> de seu pai

:focus                                input:focus             Seleciona o elemento <input> que tem foco

:in-range                           input:in-range        Seleciona elementos <input> com um valor dentro de um intervalo especificado

:invalid                              input:invalid            Seleciona todos os elementos <input> com um valor inválido

:lang(language)               p:lang(it)                  Seleciona cada elemento <p> com um valor de atributo lang começando com "it"

:last-child                          p:last-child             Seleciona todos os elementos <p> que são o último filho de seu pai

:last-of-type                     p:last-of-type         Seleciona cada elemento <p> que é o último elemento <p> de seu pai

:not(selector)                    :not(p)                    Seleciona todos os elementos que não são um elemento <p>

:nth-child(n)                       p:nth-child(2)      Seleciona cada elemento <p> que é o segundo filho de seu pai

:nth-last-child(n) p:nth-last-child(2) Seleciona cada elemento <p> que é o segundo filho de seu pai, contando a partir do último filho

:nth-last-of-type(n)             p:nth-last-of-type(2)      Seleciona cada elemento <p> que é o segundo elemento <p> de seu pai, contando a partir do último filho

:nth-of-type(n)                          p:nth-of-type(2)                          Seleciona cada elemento <p> que é o segundo elemento <p> de seu pai

:only-of-type                          p:only-of-type                          Seleciona cada elemento <p> que é o único elemento <p> de seu pai

:only-child                          p:only-child                          Seleciona cada elemento <p> que é o único filho de seu pai

:optional                          input:optional                          Seleciona elementos <input> sem atributo "obrigatório"

:out-of-range                          input:out-of-range                          Seleciona elementos <input> com um valor fora de um intervalo especificado

:read-only                          input:read-only                          Seleciona elementos <input> com um atributo "readonly" especificado

:read-write                          input:read-write                          Seleciona elementos <input> sem atributo "readonly"

:required                          input:required                          Seleciona elementos <input> com um atributo "obrigatório" especificado

:root                                  root                                 Seleciona o elemento raiz do documento

:target                          [#news](https://www.youtube.com/hashtag/news):target                          Seleciona o elemento [#news](https://www.youtube.com/hashtag/news) ativo atual (clicado em um URL que contém esse nome de âncora)

:valid                          input:valid                          Seleciona todos os elementos <input> com um valor válido

## Pseudo Elements

::after                             p::after                          inserir conteúdo após cada elemento <p>

::before                         p::before                          Inserir conteúdo antes de cada elemento <p>

::first-letter                   p::first-letter               Seleciona a primeira letra de cada elemento <p>

::first-line                      p::first-line                   Seleciona a primeira linha de cada elemento <p>

::selection                      p::selection                 Seleciona a parte de um elemento que é selecionado por um usuário

