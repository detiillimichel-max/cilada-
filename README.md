🫂Cilada📲
"Quero criar um jogo mobile baseado no clássico 'Cilada' da Estrela. Para que você desenvolva o código sem erros, siga estritamente este raciocínio lógico estruturado:

1. REPRESENTAÇÃO DO TABULEIRO:
- O tabuleiro deve ser uma matriz bidimensional fixa de tamanho X por Y (ex: 10x10).
- Cada célula da matriz inicia com o valor inteiro 0 (que significa ESPAÇO VAZIO).
- Se a célula contiver o valor 1, significa ESPAÇO OCUPADO.

2. ESTRUTURA DAS PEÇAS (POLIOMINÓS):
- Cada peça é uma forma geométrica única composta por blocos quadrados adjacentes.
- Represente cada peça como uma lista de coordenadas relativas a partir de um ponto de origem (0,0).
- Exemplo de peça em formato de 'L': [(0,0), (1,0), (2,0), (2,1)]
- Permita que a peça seja rotacionada em 90, 180 ou 270 graus antes de ser colocada, recalculando suas coordenadas.

3. ALGORITMO DE VALIDAÇÃO DE ENCAIXE (MECÂNICA CORE):
Quando o usuário arrastar uma peça e tentar soltá-la em uma célula-alvo (Linha_Alvo, Coluna_Alvo) do tabuleiro, faça a seguinte verificação ANTES de confirmar o movimento:
- Para cada coordenada (dx, dy) da peça:
    Calcule a posição final na matriz: L = Linha_Alvo + dx e C = Coluna_Alvo + dy
    A jogada é INVÁLIDA se:
    a) L ou C estiverem fora dos limites da matriz (Index Out of Bounds).
    b) Matriz[L][C] for igual a 1 (Espaço já ocupado por outra peça).
- Se todas as coordenadas passarem no teste, mude o valor dessas células na Matriz de 0 para 1 e fixe a peça ali.

4. CONDIÇÃO DE VITÓRIA E DERROTA:
- VITÓRIA: Se a quantidade de células com valor 1 for igual ao tamanho total de blocos de todas as peças disponíveis (Tabuleiro completamente preenchido).
- CILADA (DERROTA/TRAVAMENTO): Se sobrarem peças na mão do jogador, mas o algoritmo de validação retornar FALSO para absolutamente todas as posições livres restantes do tabuleiro.

Com base nesse raciocínio lógico, gere o código completo do jogo utilizando [INSERIR A TECNOLOGIA, EX: Flutter/React Native/HTML5 com Canvas]."
