# Matriz de Responsabilidades da Equipe

**Versão:** 0.1
**Status:** Em definição

## 1. Objetivo

Definir responsáveis principais por cada área do projeto, reduzir sobreposição de trabalho e evitar que responsabilidades importantes fiquem sem dono.

Uma pessoa pode atuar em mais de uma área, mas cada responsabilidade deve possuir um responsável principal.

---

## 2. Equipe

| Integrante | Áreas atuais                        |
| ---------- | ----------------------------------- |
| Rodrigo    | Organização, produção e game design |
| Gustavo    | Level design                        |
| Daniel     | Programação e música                |
| Guilherme  | Programação                         |
| Juliana    | Áudio e design                      |
| Rebeca     | Design                              |

---

## 3. Matriz de responsabilidades

| Área                              | Responsável principal              | Apoio                    | Entregável                                      | Dependências         |
| --------------------------------- | ---------------------------------- | ------------------------ | ----------------------------------------------- | -------------------- |
| Produção e organização            | Rodrigo                            | Equipe                   | Backlog, prioridades, decisões e acompanhamento | Definições da equipe |
| Game design                       | Rodrigo                            | Gustavo, Rebeca, Juliana | Regras, mecânicas e balanceamento inicial       | Playtests            |
| Level design                      | Gustavo                            | Rodrigo                  | Salas, rotas, obstáculos e situações de stealth | Mecânicas funcionais |
| Programação de gameplay           | A definir entre Daniel e Guilherme | Outro programador        | Movimento, combate e interação do jogador       | Game design          |
| Programação de IA e sistemas      | A definir entre Daniel e Guilherme | Outro programador        | Inimigos, stealth, run e sistemas relacionados  | Gameplay base        |
| Sistema de consequências da morte | A definir entre Daniel e Guilherme | Rodrigo                  | Registro e aplicação das alterações entre runs  | Run, level design    |
| Música                            | Daniel                             | Juliana                  | Música necessária para o protótipo              | Direção do jogo      |
| Efeitos sonoros                   | Juliana                            | Daniel                   | Sons de combate, alerta, morte e interação      | Gameplay             |
| Direção visual                    | A definir                          | Juliana, Rebeca          | Identidade visual mínima do protótipo           | Conceito             |
| Arte de personagens               | A definir                          | Juliana, Rebeca          | Player e inimigos                               | Direção visual       |
| Arte de cenário                   | A definir                          | Juliana, Rebeca, Gustavo | Tiles, obstáculos e elementos de sala           | Level design         |
| UI/UX                             | A definir                          | Juliana, Rebeca, Rodrigo | HUD, menus e feedback visual                    | Gameplay             |
| Playtesting                       | Rodrigo organiza                   | Todos                    | Sessões de teste e registro dos resultados      | Build jogável        |
| Gerenciamento de builds           | A definir                          | Programadores            | Builds de teste                                 | Projeto estável      |
| Revisão de Pull Requests          | Daniel e Guilherme                 | Rodrigo quando aplicável | Revisão técnica antes de merge                  | GitHub               |
| Documentação                      | Rodrigo                            | Responsável de cada área | Registro de decisões e documentação mínima      | Trabalho concluído   |

---

## 4. Responsabilidades específicas

### Rodrigo

Responsável por:

* organização;
* acompanhamento;
* backlog;
* game design;
* registro de decisões;
* organização dos playtests.

Não deve centralizar decisões técnicas que pertencem aos programadores ou decisões artísticas que pertencem aos responsáveis visuais.

### Gustavo

Responsável por:

* construção das salas;
* rotas;
* posicionamento de obstáculos;
* posicionamento inicial de inimigos;
* situações de stealth;
* integração entre level design e consequências das mortes.

### Daniel e Guilherme

Responsáveis pela programação.

Antes da produção principal, devem dividir entre si pelo menos:

* gameplay do jogador;
* combate;
* IA;
* stealth;
* estrutura da run;
* sistema de consequências das mortes.

A divisão deve evitar que os dois trabalhem frequentemente nos mesmos arquivos.

### Daniel

Além da programação, será responsável pela música.

A música não deve bloquear tarefas prioritárias de programação.

### Juliana

Responsável por áudio e participante das áreas de design.

Responsabilidades confirmadas:

* efeitos sonoros;
* feedback sonoro;
* apoio visual.

A divisão exata da parte visual ainda precisa ser definida.

### Rebeca

Responsável por design.

A responsabilidade específica entre:

* personagens;
* cenário;
* UI;
* conceitos;
* animação;

ainda precisa ser definida.

---

## 5. Regra de responsabilidade

Para cada tarefa:

**Responsável principal:** pessoa que garante que a tarefa chegue ao estado de concluída.

**Apoio:** pessoas que podem colaborar, revisar ou fornecer assets.

Ter apoio não divide a responsabilidade principal.

---

## 6. Riscos atuais

### Sobrecarga de Daniel

Daniel acumula programação e música.

**Prevenção:** programação do protótipo deve ter prioridade sobre produção musical extensa.

### Programadores editando os mesmos sistemas

Daniel e Guilherme podem gerar conflitos frequentes no Git se a divisão técnica não estiver clara.

**Prevenção:** separar ownership inicial dos sistemas.

### Área visual ainda indefinida

Juliana e Rebeca possuem responsabilidades descritas apenas como "design".

**Prevenção:** definir quem assume principalmente personagens, cenários, UI e animação antes da produção de assets.

---

## 7. Responsabilidades ainda pendentes

Precisam ser definidas antes de suas respectivas tarefas começarem:

* divisão técnica entre Daniel e Guilherme;
* direção visual;
* arte de personagens;
* arte de cenário;
* animação;
* UI/UX;
* gerenciamento de builds.
