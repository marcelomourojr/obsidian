
# DNS


![[Pasted image 20250827142433.png]]


**Os registros de recursos (RRs) são o banco de dados do DNS. São compostos por tuplas de cinco campos:**


<font color="#f79646">Nome:</font> chave de pesquisa primária para atender as consultas; 

<font color="#f79646">Tempo_vida (TTL):</font> tempo que deve permanecer em cache (em segundos); 

<font color="#f79646">Classe:</font> geralmente IN (Internet);  

<font color="#f79646">Tipo: </font>SOA, A, AAAA etc. (tabela a seguir); 

<font color="#f79646">Valor:</font> número, nome de domínio ou string ASCII.

![[Pasted image 20250827142917.png]]

Uma <font color="#9bbb59">resposta autoritativa </font>de um servidor é a garantia de estar <u>atualizada</u>, enquanto uma resposta <font color="#c0504d">não-autoritativa</font> pode estar <u>desatualizada</u>.