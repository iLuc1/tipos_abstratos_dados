# Tipos Abstratos de Dados
Estudos de aplicações referentes a tipos abstratos de dados

## Árvore
A árvore é um tipo abstrato de dados muito utilizados em sistemas de arquivos, páginas na internet, 
árvore genalógicas, banco de dados e estruturas organizacionais.

![Árvore](arvore.gif)

Uma árvore é uma estrutura de dados bidirecional não linear, ou seja, cada elemento da árvore pode ter mais 
que um predecessor e mais que um sucessor.

Essa estrutura de dados armazena os elementos de forma hierárquia, isso quer dizer que com exceção do topo
todo elemento possui um pai, e pode ter 0 ou mais filhos - a quantidade de filhos podem ser limitados em casos
de árvores binárias, por exemplo.

O elemento do topo é conhecido como raiz e cada nó pode ser externo ou interno. Os nós externos são aqueles que não
possuem filhos(são as pontas das arvores) e podem também ser chamados de folhas, já os nós internos são aqueles
que possuem filhos.

### Ancestralidade
O ancestral de um nó é tanto ancestral do pai quanto do nó pai.

### Operações
A árvore geralmente pode possuir as seguintes funções:

* Raiz: retorna a raiz da árvore(entrada: nenhum, saída: posição)
* Pai: retorna o pai de v, se v for a raiz retorna erro(entrada: posição, saída: posição)
* Filhos: retorna os filhos de um nó(entrada: posição, saída: lista)
* Verifica interno: checa se um nó é interno(entrada: posição, saída: booleano)
* Verifica externo: checa se um nó é externo(entrada: posição, saída: booleano)
* Verifica raíz: checa se um nó é raiz(entrada: posição, saída: booleano)
* Tamanho: retorna o número de nós da raiz(entrada: nenhum, saída: inteiro)
* Elementos: retorna uma lista com todos os nós(entrada: nenhum, saída: lista)
* Atualiza elemento: retorna o elemento armazenado em v e substitui por e(entrada: posição e objeto, saída: objeto)
* Insere: insere um elemento em uma raiz(entrada: raiz e objeto, saída: nenhuma)

### Nível ou profundidade
Sendo v um nó de uma árvore T, a profundidade de v é o número de ancestrais do mesmo. Ou seja, é o comprimento de v
até a raiz, sendo que a raiz equivale a 0. 
A profundidade de um nó v pode ser definida de forma recursiva, caso v for a raiz, então a profundidade é 0. Nos outros casos
a profundidade será 1 a mais que a profundidade do pai de v.

### Altura
A altura de v é o comprimento mais longo de v até uma folha, sendo que a altura de uma folha é 0.
Se v é um nó externo, então a altura dele será 0, caso o contrário a altura de v será o maior comprimento até chegar em uma folha.
A altura de uma árvore é definida pela altura de uma raiz.

### Percurso 
Percorrer uma árvore significa acessar todos os nós da mesma.

#### Caminho pré-fixado
0 caminho pré-fixado é quando os nós começam a ser percorridos a partir do pai, formando uma lista onde os pais aparecem antes dos filhos.

#### Caminho pós-fixado
O oposto do pré-fixado, listando os filhos antes dos pais, sendo a raiz a última a aparecer.