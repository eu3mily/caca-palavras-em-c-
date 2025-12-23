# caca-palavras-em-c-
Recordação do meu projeto universitário final na cadeira de LP1 (linguagem de programação 1). Esse projeto contempla um jogo de caça palavras simples em C, com manipulação de matrizes 2D e 3D, arquivos, e criatividades de acordo com o jogo comum. :)


--> OBJETIVO
Encontrar todas as palavras escondidas na matriz de letras, com interface no terminal, informando a palavra e a linha inicial correta.

--> FUNCIONALIDADES
- Três níveis de dificuldade:
  Fácil (10x10 – 3 palavras) 1 ponto
  Médio (15x15 – 5 palavras) 2 pontos
  Difícil (20x20 – 7 palavras) 3 pontos
- Palavras posicionadas na horizontal, vertical e diagonal
- Substituição das palavras encontradas por asteriscos ('*')
- Sistema de dicas (máximo de duas por jogo)
- Validação de jogadas (acerto, erro e repetida)
- Sistema de resumo da partida
- Sistema de score acumulativo
- Salvamento do resultado final em arquivo

--> ESTRUTURA DO PROJETO
main.c              Arquivo principal
funcoesdojogo.c     Implementação das funções
jogo.h              Header (cabeçalho) com structs, enums e protótipos
palavras.txt        Palavras utilizadas no jogo
replay.txt          Replay da partida
resultado.txt       Resultado final do jogo
scorelog            Score acumulativo 
scoretotal.txt      Score total 

--> COMANDOS DO JOGO
- Digitar: PALAVRA E LINHA EM QUE ELA COMEÇA (ex: a intenção é que o jogador digite 'BAHIA 3', para representar a palavra 'BAHIA' que começa na linha 3)
- SAIR 0 → encerra o jogo (e dá a opção de ver o resumo do jogo)
- DICA 0 → recebe uma dica (a dica fala a primeira letra da palavra e a linha onde ela está escondida, com a limitação de duas por jogo)

--> ** OBS. RECURSO DE TESTE:
A função: "void mostrarCoordenadas(Palavra palavras[], int qtd);", foi criada como um recurso de teste para nos ajudar a debuggar e testar o jogo, é ela que mostra exatamente as coordenadas de onde as palavras estarão escondidas no tabuleiro 

Para o jogo rodar como deve (o jogador obviamente não pode saber onde as palavras estão) , deixaremos essa função comentada(ocultada), mas caso precise ajustar algo, para facilitar a visualização das palavras, a deixaremos visivel novamente.


