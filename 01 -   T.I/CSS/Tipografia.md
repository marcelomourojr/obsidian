# Tipografia

## Medidas Absolutas:

cm, mm, in, px, pt, pc 

## Medidas Relativas: 

em -> relativo ao tamanho natural da fonte 
ex -> relativo a altura x da fonte 
rem -> tipo em, mas relativo a fonte configurada no body 
vw -> relativo a largura da view port 
vh -> relativo a altura da view port 
% -> porcentagem 

**Recomendação w3c: "px" ou "em"** 

**Altura padrão: 16px ou 1em**



## Peso (negrito):

- fonte mais cheia (negrito) ou fina

- não serve para fontes simples (arial, verdana, times,...)

- serve pra fontes como Work Sans (import google)

  

font-weight: nome ou número;    

  

   nome:                           número:
   
- lighter número:         - 100    - 500   - 900

- normal                      - 200    - 600

- bold                          - 300   - 700

- bolder                       - 400   - 800

  

## Estilo (itálico):

  

font-style: valor;                   valor:  - normal

.                                                         - italic

  

Decoração (sublinhado):

text-decoration: underline;

  
Shorthand font: simplificando fontes.

   Ex: 
   
- font-family: 'Work Sans', sans-serif;

- font-weight: bolder;

- font-size: 3em;

 - font-style: italic;


Simplificando:

font:  italic  bolder  3em  'Work Sans', sans-serif;


A sequência deve ser:

font-style   ->   font-weight   ->   font-size   ->   font-family;
  

Não precisa ter todas as propriedades, mas a sequência deve ser seguida;

  Ex: font:  bold  2em  'Work Sans';