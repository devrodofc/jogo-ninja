# Escopo do Protótipo — 1 HP

**Versão:** 0.1
**Status:** Em definição
**Objetivo:** definir o menor escopo capaz de validar a proposta principal do jogo.

## 1. Objetivo do protótipo

Validar se a combinação de:

* 1 HP;
* morte instantânea;
* stealth;
* combate;
* reinício da tentativa;
* consequências geradas pelas mortes anteriores;

cria uma experiência interessante de tensão, estratégia, precisão e adaptação.

O protótipo não precisa representar o jogo completo.

---

## 2. Obrigatório — P0/P1

Funcionalidades necessárias para validar a ideia.

### Jogador

* movimentação top-down;
* 1 HP;
* morte ao receber dano;
* combate corpo a corpo;
* combate à distância;
* feedback claro de morte.

### Inimigos

Pelo menos um tipo de inimigo: ninja zumbi.

Comportamentos mínimos:

* patrulha;
* detecção do jogador;
* estado de alerta;
* perseguição;
* ataque;
* morte.

### Furtividade

* possibilidade de evitar detecção;
* obstáculos que bloqueiem visão;
* feedback que permita entender se o jogador foi detectado.

### Estrutura da tentativa

* início de uma tentativa;
* progressão por uma pequena sequência de áreas;
* morte;
* reinício;
* condição simples de vitória.

A decisão entre reiniciar toda a run ou apenas um conjunto de salas permanece aberta.

### Sistema de consequências da morte

O jogo deve conseguir registrar informações relevantes sobre a morte, como:

* local;
* causa;
* sala;
* categoria do efeito.

Na tentativa seguinte, pelo menos uma consequência deve poder ser criada a partir desse registro.

Para validar o sistema, o protótipo precisa de apenas **2 ou 3 tipos diferentes de consequência**.

Os efeitos específicos ainda serão definidos.

### Level design

* poucas salas pequenas;
* caminhos que permitam stealth e combate;
* obstáculos;
* áreas onde as consequências das mortes possam alterar a abordagem do jogador.

### Interface

Somente o necessário para:

* iniciar;
* reiniciar;
* comunicar morte;
* comunicar vitória;
* apresentar informações indispensáveis ao gameplay.

### Áudio

Somente sons necessários para leitura do gameplay, como:

* ataque;
* morte;
* alerta;
* detecção;
* interação importante.

Música é desejável, mas não deve bloquear a validação do protótipo.

---

## 3. Desejável — P2

Implementar apenas se o núcleo estiver funcionando e houver tempo.

* mais de um tipo de inimigo;
* variedade maior de armas;
* diferentes tipos de consequências de morte;
* efeitos visuais mais elaborados;
* música dinâmica;
* diferentes rotas pelas salas;
* pequenas variações entre runs;
* sistema simples de itens;
* melhorias temporárias;
* tela simples de fim de run;
* tutorial integrado ao gameplay.

---

## 4. Ideias futuras — P3/P4

Registrar, mas não implementar durante a primeira validação.

* grande variedade de armas;
* vários tipos de ninjas zumbis;
* bosses;
* progressão permanente;
* árvore de habilidades;
* sistemas complexos de builds;
* geração procedural avançada;
* múltiplas regiões;
* narrativa extensa;
* personagens adicionais;
* modos alternativos.

---

## 5. Fora do escopo atual

* multiplayer;
* coop para dois jogadores;
* PvP;
* sistemas online;
* matchmaking;
* contas;
* servidores;
* campanha extensa;
* mundo aberto;
* crafting complexo;
* inventário complexo;
* publicação comercial completa;
* suporte simultâneo garantido para todas as plataformas.

Android permanece fora do primeiro escopo até que a equipe decida se o jogo será projetado para controles por toque.

---

## 6. Critérios mínimos para considerar o protótipo jogável

O protótipo estará pronto para playtest quando um jogador conseguir:

1. iniciar uma tentativa;
2. movimentar-se e navegar pelas salas;
3. evitar ou enfrentar inimigos;
4. matar inimigos;
5. morrer com um único golpe;
6. reiniciar a tentativa;
7. encontrar uma consequência causada por uma morte anterior;
8. adaptar sua abordagem por causa dessa consequência;
9. alcançar uma condição de vitória.

---

## 7. Critérios de validação

Ainda precisam ser aprovados pela equipe.

Sugestões para o primeiro playtest:

* o jogador entende por que morreu;
* o jogador percebe as consequências das mortes anteriores;
* as consequências alteram alguma decisão;
* o jogador entende quando está sendo detectado;
* morte e reinício não interrompem excessivamente o ritmo;
* stealth e combate oferecem alternativas reais;
* o jogador demonstra interesse em tentar novamente.

---

## 8. Regras de controle de escopo

Uma nova funcionalidade só entra no protótipo se:

1. for necessária para testar a hipótese principal; ou
2. resolver um problema identificado durante playtest.

Caso contrário, deve ser registrada como P2, P3 ou P4.

Antes de adicionar:

* nova arma;
* novo inimigo;
* nova mecânica;
* nova categoria de consequência;
* novo sistema de progressão;

a equipe deve verificar se o conteúdo atual já foi testado.

---

## 9. Decisões ainda pendentes

* reinício da run completa ou conjunto de salas;
* tamanho aproximado de uma run;
* número de salas do primeiro protótipo;
* primeiras consequências de morte;
* primeiras armas;
* objetivo final da run;
* plataforma principal;
* existência ou não de progressão permanente.
