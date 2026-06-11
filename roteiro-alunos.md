# Roteiro para os Alunos: Jogo 3D em Unity para Android

## Objetivo

Desenvolver em grupo um jogo 3D simples em Unity, testado primeiro no computador e depois em smartphone Android.

O jogo nao precisa ser grande. Ele precisa ser **jogavel, compreensivel e funcional**.

## Regra de ouro

Antes de pensar em graficos bonitos, faca o jogo funcionar:

1. o jogador entra na cena;
2. o jogador consegue se mover;
3. a camera mostra bem a acao;
4. existe um objetivo claro;
5. o jogo reconhece vitoria ou derrota;
6. o projeto roda no celular.

## Escopo recomendado

Escolha uma ideia pequena:

- coletar 5 objetos antes do tempo acabar;
- escapar de uma sala;
- atravessar um percurso com obstaculos;
- encontrar uma chave e abrir uma porta;
- desviar de inimigos simples;
- resolver um puzzle em uma unica fase.

Evite ideias grandes:

- mundo aberto;
- multiplayer;
- muitas fases;
- historia longa;
- sistema de loja;
- inventario complexo;
- combate com muitos inimigos;
- graficos realistas.

## Configuracao inicial

Padrao tecnico da disciplina:

- template do projeto: `3D (Built-in Render Pipeline)`;
- pipeline: `Built-in Render Pipeline`;
- plataforma alvo: Android;
- cena principal: `MainScene`.

Cada grupo deve criar:

- uma pasta `Assets/Scenes`;
- uma pasta `Assets/Scripts`;
- uma pasta `Assets/Prefabs`;
- uma pasta `Assets/Materials`;
- uma pasta `Assets/Audio`;
- uma cena principal chamada `MainScene`.

Nome do projeto:

```text
GrupoNome_Jogo3D
```

## Entrega 1: Projeto e GDD reduzido

O grupo deve entregar:

- nome do jogo;
- integrantes;
- genero;
- objetivo do jogador;
- controles;
- condicao de vitoria;
- condicao de derrota, se houver;
- rascunho da tela ou mapa da fase.
- print do projeto Unity criado;
- print do acesso ao Unity Cloud Studio;
- print de um personagem ou animacao escolhida no Mixamo.

Modelo rapido:

```text
Titulo:
Genero:
Pitch em 3 linhas:
O jogador controla:
Objetivo:
Como vence:
Como perde:
Controles:
Elementos 3D principais:
Responsavel pelo build Android:
Personagem/personagens previstos:
Animacao inicial prevista:
```

## Entrega 2: Movimento 3D

O jogo deve ter:

- chao;
- jogador;
- camera;
- movimento;
- colisao basica.

Controles minimos no Editor:

- `WASD` ou setas para mover;
- mouse ou camera fixa;
- tecla `Espaco` se houver pulo.

Para mobile, o grupo pode escolher:

- joystick virtual simples;
- botoes na tela;
- movimento automatico com toque para virar;
- jogo em primeira pessoa com controles simples.

## Entrega 3: Primeiro teste Android

O grupo deve tentar gerar o primeiro build Android cedo.

Esse build pode ser simples e incompleto. O objetivo e validar que:

- o projeto compila;
- o celular reconhece o APK;
- a cena abre no aparelho;
- a performance inicial permite continuar o desenvolvimento.

Evidencias da entrega:

- APK;
- video curto do jogo abrindo no celular;
- print do Unity mostrando o status do build.

## Entrega 4: Objetivo e vitoria

O jogo deve ter pelo menos uma regra completa.

Exemplos:

- coletar 5 moedas mostra "Vitoria";
- chegar na porta final termina a fase;
- sobreviver 60 segundos vence;
- tocar em obstaculo reinicia a cena;
- encontrar 3 pecas ativa um portal.

## Entrega 5: Obstaculos e desafio

Adicionar dificuldade simples:

- obstaculos parados;
- plataforma movel;
- inimigo que patrulha;
- tempo limite;
- area perigosa;
- objeto que diminui pontuacao.

Nao precisa de IA complexa. O desafio deve ser claro e testavel.

## Entrega 6: Audio, UI e feedback

Adicionar:

- texto de pontuacao ou objetivo;
- som de coleta, dano ou vitoria;
- tela simples de fim;
- botao de reiniciar;
- feedback visual quando o jogador acerta ou erra.

## Entrega 7: Otimizacao para mobile

Verificar:

- poucos objetos na cena;
- luzes em excesso removidas;
- texturas muito grandes evitadas;
- particulas usadas com moderacao;
- sombras pesadas reduzidas;
- APK testado em pelo menos um celular.

## Entrega final

O grupo deve entregar:

- projeto Unity ou link do projeto;
- APK Android;
- video de gameplay de 1 a 3 minutos;
- GDD atualizado;
- lista de assets externos usados;
- breve divisao de tarefas do grupo.

