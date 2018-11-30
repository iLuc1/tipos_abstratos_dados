# Tipos Abstratos de Dados
Estudos de aplicações referentes a tipos abstratos de dados

#### Árvore
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

####### Ancestralidade
O ancestral de um nó é tanto ancestral do pai quanto do nó pai.

####### Operações
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
