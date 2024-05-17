# Árvore de Busca para Jogo da Velha em Python 🐍

Este projeto consiste em uma implementação de uma estrutura de árvore de busca para o jogo da velha em Python. Ele fornece uma estrutura básica para representar os estados do jogo, gerar a árvore de busca e realizar a busca por meio de diferentes algoritmos de resolução de problemas.

## Estrutura de Dados

O jogo da velha é representado por uma matriz 3x3, onde cada célula pode conter 'X', 'O' ou estar vazia (' '). A estrutura de dados da árvore é implementada com a classe `Node`, que possui os seguintes atributos:

- `state`: Representação do estado atual do jogo.
- `parent`: Nó pai na árvore.
- `action`: Ação que levou a este estado.
- `children`: Lista de nós filhos.

## Funcionalidades

### Estado Inicial

O estado inicial do jogo é uma matriz 3x3 onde todas as células estão vazias.

### Ações

As ações possíveis em um estado são representadas pelas coordenadas (linha, coluna) onde um jogador pode fazer sua jogada. Por exemplo, a ação (0, 0) indica que o jogador pode jogar na primeira linha e primeira coluna.

### Modelo de Transição

O modelo de transição é implementado pela função `result`, que recebe um estado, uma ação e um jogador, e retorna o novo estado após a realização da ação pelo jogador.

### Teste de Objetivo

O teste de objetivo ainda não está implementado explicitamente neste projeto, mas pode ser feito verificando se um jogador ganhou ou se o tabuleiro está completamente preenchido (empate).

### Custo de Caminho

Não há uma função de custo de caminho definida explicitamente neste projeto, uma vez que estamos apenas construindo a árvore de busca. O custo geralmente é tratado em algoritmos de busca como A*, onde é a soma do custo de cada ação, mas para o jogo da velha pode ser tratado como constante, já que todas as ações têm o mesmo custo.

## Utilização

Para usar a estrutura de árvore de busca, basta instanciar a classe `TicTacToeTree` e chamar o método `generate_tree` para gerar a árvore de busca. Em seguida, você pode usar diferentes algoritmos de busca para encontrar a melhor jogada.

```python
game_tree = TicTacToeTree()
game_tree.generate_tree(game_tree.root, 'X')

```

<hr>
<p align="center">2024 - Maria de Fátima Nunes Alves</p>
