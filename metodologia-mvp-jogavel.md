# Metodologia: MVP Jogavel por Marcos

## Visao geral

A metodologia adotada para o trabalho e o **MVP jogavel por marcos**.

MVP significa **Minimum Viable Product**, ou Produto Minimo Viavel. No contexto da disciplina, isso quer dizer: criar primeiro a menor versao possivel do jogo que ja possa ser jogada do inicio ao fim.

Depois que essa versao minima funciona, o grupo evolui o projeto por etapas.

## Por que usar esta metodologia

Esta metodologia e adequada para projetos iniciantes em Unity porque:

- facilita a organizacao do grupo;
- evita escopo grande demais;
- permite avaliacao semanal;
- coloca a jogabilidade antes do visual;
- permite testar Android cedo;
- torna o progresso facil de demonstrar em video.

## Regra principal

O grupo deve sempre priorizar esta ordem:

1. funcionar;
2. ser jogavel;
3. ser compreensivel;
4. rodar no Android;
5. ficar bonito.

Visual, audio e efeitos sao importantes, mas entram depois que o jogo ja possui uma estrutura jogavel.

## Marcos do projeto

### Marco 1: Ideia e escopo

O grupo define:

- titulo;
- genero;
- objetivo;
- controles;
- condicao de vitoria;
- condicao de derrota;
- responsavel pelo build Android.

Resultado esperado: GDD reduzido.

### Marco 2: Prototipo de movimento

O grupo cria:

- cena principal;
- chao;
- jogador;
- camera;
- movimento;
- colisao basica.

Resultado esperado: video curto no Unity Editor.

### Marco 3: Primeira validacao Android

O grupo configura:

- plataforma Android;
- orientacao da tela;
- build settings;
- primeiro APK de teste.

Resultado esperado: APK ou video do projeto abrindo no celular.

### Marco 4: Regra principal

O grupo implementa:

- objetivo coletavel, porta, chegada, timer ou puzzle;
- pontuacao ou progresso;
- condicao de vitoria.

Resultado esperado: o jogo ja tem inicio, acao e fim.

### Marco 5: Desafio

O grupo adiciona pelo menos um elemento de dificuldade:

- obstaculo;
- inimigo simples;
- area perigosa;
- tempo limite;
- plataforma movel;
- penalidade.

Resultado esperado: video mostrando sucesso e erro/derrota.

### Marco 6: Interface e feedback

O grupo adiciona:

- pontuacao ou objetivo na tela;
- mensagem de vitoria;
- mensagem de derrota ou reinicio;
- som;
- feedback visual.

Resultado esperado: gameplay mais claro para o jogador.

### Marco 7: Otimizacao mobile

O grupo revisa:

- quantidade de objetos;
- luzes;
- sombras;
- tamanho de texturas;
- particulas;
- tamanho do APK;
- execucao no celular.

Resultado esperado: versao mobile demonstravel.

### Marco 8: Entrega final

O grupo entrega:

- projeto Unity;
- APK Android;
- video de gameplay;
- GDD atualizado;
- creditos de assets;
- divisao de tarefas.

## Padrao tecnico da disciplina

Todos os grupos devem usar:

- Unity LTS indicada pelo professor;
- template `3D (Built-in Render Pipeline)`;
- pipeline `Built-in Render Pipeline`;
- cena principal chamada `MainScene`;
- projeto configurado para Android;
- pastas organizadas em `Scenes`, `Scripts`, `Prefabs`, `Materials` e `Audio`.

## Definicao de pronto

Uma entrega esta pronta quando:

- abre no Unity sem erros vermelhos;
- possui a funcionalidade combinada para o marco;
- pode ser demonstrada em video;
- esta organizada no projeto;
- foi testada pelo grupo antes da entrega.

