# Async-Reflex-Game
nUSP: 8532269 e 10550198
Jogo implementado com técnicas assíncronas de JavaScript.


Parte 1:
O que foi adicionado ao jogo original: 
  - Cor de fundo trocada
  - Scores para os jogadores
  - Reinicia os scores quando a condição de vitória for alcançada (clearInterval)
  - Adicionada quantidade de rounds para um jogador vencer a partida (5 rounds)
  - Adicionada tela de vencedor (Fim de jogo)
  - Efeito de "piscar" na escrita do vencedor do jogo (setInterval)
  - Efeito de "chacoalhar" na escrita do vencedor do jogo (setInterval)


Parte 2:
Diferenças de abordagens em relação ao primeiro jogo: 
        - O setTimeout da função start() é implementado em uma Promise (startTimeoutPromise())
        - Todos os setInterval são implementados com Promises
        - A lógica do jogo em si não foi alterada, porém com o uso de Promises, as lógicas das funções que usam setInterval e setTimeout tiveram que ser modificadas, retornando um array contendo a referência (ou identificador) para o setInterval ou setTimeout executado