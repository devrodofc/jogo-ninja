Game Design Document — Protótipo 1 HP

Versão: 0.1
Status: Em definição
Engine: Godot
Formato: Jogo 2D top-down
Modo: Single-player

1. Conceito

Jogo roguelite/roguelike furtivo top-down em que o jogador controla um ninja que possui apenas 1 HP.

Qualquer dano recebido causa a morte do personagem e inicia uma nova tentativa.

A principal característica do jogo é que as mortes anteriores podem modificar tentativas futuras.

Dependendo da causa, local ou circunstância da morte, uma alteração poderá aparecer naquele ponto em uma run posterior.

Essas alterações podem:

- beneficiar o jogador;
- prejudicar o jogador;
- beneficiar inimigos;
- prejudicar inimigos;
- modificar o ambiente;
- criar obstáculos;
- criar oportunidades estratégicas;
- gerar itens, poderes ou outros efeitos.

Os efeitos específicos ainda serão definidos.

2. Fantasia do jogador

O jogador assume o papel de um ninja extremamente vulnerável, mas rápido e perigoso.

Ele deve observar o ambiente, planejar sua abordagem e executar suas ações com precisão.

O objetivo é criar situações em que combate direto seja possível, mas nem sempre seja a melhor alternativa.

3. Pilares de design

Tensão

Um único erro pode terminar a tentativa.

Precisão

Movimentação e combate devem responder de maneira previsível e precisa.

Velocidade

O jogador deve conseguir executar rapidamente um plano depois de decidir como agir.

Estratégia

Posicionamento, armas, ambiente e comportamento dos inimigos devem influenciar as decisões.

Furtividade

Evitar ser detectado deverá ser uma alternativa importante ao combate direto.

4. Loop principal

1. Entrar em uma área.
2. Observar inimigos e ambiente.
3. Planejar uma abordagem.
4. Avançar furtivamente ou combater.
5. Superar a área.
6. Continuar a run.

Caso o jogador seja atingido:

1. O jogador morre.
2. A morte é registrada.
3. A tentativa é reiniciada.
4. Uma consequência relacionada à morte poderá aparecer em uma tentativa futura.
5. O jogador adapta sua estratégia às mudanças.

5. Combate

O combate será uma mistura de:

- corpo a corpo;
- ataques à distância.

A intenção futura é possuir diferentes armas.

Para o primeiro protótipo, a quantidade e os tipos de armas ainda não estão definidos.

6. Inimigos

Os primeiros inimigos planejados são ninjas zumbis.

Eles deverão conseguir, inicialmente:

- patrulhar;
- perceber o jogador;
- reagir à presença do jogador;
- perseguir;
- atacar;
- morrer.

Tipos adicionais de inimigos serão definidos somente após a validação da mecânica principal.

7. Sistema de morte

O jogador possui exatamente 1 HP.

Qualquer ataque válido recebido causa morte.

A morte deve possuir:

- causa identificável;
- posição registrada;
- feedback claro;
- reinício rápido.

A morte não funciona apenas como punição. Ela também alimenta o sistema de alterações entre tentativas.

8. Consequências das mortes

O sistema deve conseguir associar uma morte a informações como:

- posição;
- sala;
- causa;
- tipo de dano;
- contexto relevante.

Essas informações poderão gerar alterações em runs seguintes.

Exemplos conceituais:

- alterações físicas no cenário;
- áreas perigosas;
- obstáculos;
- vantagens;
- desvantagens;
- poderes;
- itens.

Esses exemplos representam possibilidades de design e não funcionalidades aprovadas para implementação.

9. Estrutura da run

Ainda não definido.

Precisamos decidir se uma morte:

- reinicia somente um conjunto de salas;
- reinicia toda a run.

A duração e quantidade de salas também permanecem abertas.

10. Progressão

Ainda não definido.

Possibilidades futuras incluem:

- mudanças causadas pelas mortes;
- armas encontradas durante a run;
- melhorias temporárias;
- progressão permanente.

Nenhuma dessas opções está aprovada atualmente.

11. Multiplayer

O protótipo será single-player.

Modo cooperativo para dois jogadores permanece como possibilidade futura e não faz parte do escopo atual.

12. Plataforma

Plataformas consideradas:

- Windows;
- Linux;
- macOS;
- navegador;
- Android.

A plataforma principal de desenvolvimento ainda precisa ser oficialmente definida.

13. Hipótese do protótipo

Proposta atual:

A combinação de morte instantânea, furtividade e alterações causadas pelas mortes anteriores pode criar um ciclo interessante de aprendizado, adaptação e estratégia.

A hipótese ainda deverá ser validada e refinada pela equipe.

14. O que o primeiro protótipo precisa descobrir

O protótipo deverá ajudar a responder principalmente:

- O sistema de 1 HP é divertido ou apenas frustrante?
- O jogador entende por que morreu?
- O reinício incentiva uma nova tentativa?
- Stealth e combate funcionam juntos?
- As consequências das mortes realmente influenciam novas estratégias?
- Encontrar novamente uma alteração causada por uma morte anterior é interessante?
- O jogador percebe que suas runs anteriores estão modificando o jogo?

15. Questões em aberto

- Nome do jogo.
- Estrutura completa da run.
- Quantidade de salas.
- Progressão permanente ou somente por run.
- Funcionamento exato das consequências das mortes.
- Limite de consequências simultâneas.
- Tipos de armas.
- Forma de adquirir armas.
- Tipos adicionais de inimigos.
- Objetivo final de uma run.
- Direção artística.
- Plataforma principal.