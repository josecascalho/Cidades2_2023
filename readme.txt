1. O objetivo deste exercício é perceber como pode ser feita uma
pesquisa em profundidade e largura de forma muito simples, obedecendo ao
algoritmo apresentado na sala de aula:
"
Inicia um nó fronteira que contém o estado inicial
- Inicia um conjunto de nós explorados, vazio
- Repete:
–- Se a fronteira está vazia, não há solução
–- Remove o nó da fronteira
–- Se o nó corresponde ao objetivo, retorna com solução
–- Adiciona o nó ao conjunto de nós explorados
–- Expande o nó, adicionando os nós resultantes à fronteira se
eles ainda não estão na fronteira ou no conjunto de nós
explorados
"

Em sala de aula, iremos estudar o código, criar uma fila, estudar as diferenças entre a utilização de ambas as estruturas de dados como suporte à pesquisa.

Os alunos têm de realizar as seguintes tarefas como TPC:
(a) Identificar o tipo de pesquisa utilizando uma pilha (stack)
(b) Associar as etapas do algoritmo apresentado em cima ao local do código
(c) Criar um novo ficheiro cities2.conf onde se altera a ordem da disposição das cidades
de forma a que a pesquisa com stack resulte numa solução diferente
(d) Testar o algoritmo agora utilizando uma fila (queue)
(e) Arranjar um novo exemplo com uma nova cidade de partida e de chegada e explicar as soluções
obetidas, adicionando novas cidades a um ficheiro de configuração cities3.conf e usando
tanto uma pilha como uma fila.


2. Mapa utilizado no exemplo das cidades cities.conf

***SUL*** (até Leiria) - adicionado
Leiria <-> Aveiro (115)
Leiria <-> Coimbra (67)
Leiria <-> Santarem (90)
Santarem <-> Lisboa (78)
Lisboa <-> Evora (150)
Lisboa <-> Setubal (50)
Setubal <-> Evora (103)
Evora <-> Beja (78)
Setubal <-> Beja (142)
Beja <-> Faro (152)
Setubal <-> Faro (249)

***NORTE*** (Coimbra para cima) - não adicionado
Porto <-> Vila Real (116)
Porto <-> Viseu (133)
Porto <-> Aveiro (68)
Porto <-> Braga (53)
Porto <-> Viana do Castelo (71)
Aveiro <-> Coimbra (68)
Aveiro <-> Viseu (95)
Braga <-> Viana do Castelo (48)
Braga <-> Vila Real (106)
Viseu <-> Guarda (85)
Viseu <-> Vila Real (65)
Viseu <-> Coimbra (96)
Guarda <-> Braganca (202)
Vila Real <-> Braganca (137)

3. Exemplo de mapa utilizado para cities_heuristic.conf
No cities_heuristic.conf existem dois tipos de lista, connections e heuristic. Assim, é possível
aceder aos dados de uma heurístic para aplicar uma procura não cega. Este "cities2.conf" será
discutido na 3ª aula prática.