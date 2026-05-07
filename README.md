# Trilha Unity 3D + Mobile

Material de apoio para a disciplina **Computacao Grafica e Realidade Virtual**.

Este pacote organiza a trilha pratica de desenvolvimento de um jogo 3D em Unity com validacao em smartphone Android. O objetivo e conduzir os grupos por um processo completo de producao: concepcao, prototipacao, implementacao de regras, testes, otimizacao e apresentacao final.

## Proposta didatica

A disciplina trabalha com desenvolvimento incremental. Cada grupo deve construir um jogo pequeno, funcional e testavel, evoluindo por entregas semanais.

A metodologia adotada e: **MVP jogavel por marcos**. Primeiro o grupo entrega uma versao minima jogavel; depois adiciona controles mobile, desafio, interface, audio e otimizacao.

## Estrategia de desenvolvimento

### 1. Padronizar o projeto

Cada grupo deve iniciar com um projeto 3D simples usando a versao LTS indicada pelo professor.

Configuracao base:

- template: `3D (Built-in Render Pipeline)`;
- pipeline: `Built-in Render Pipeline`;
- plataforma alvo: Android;
- orientacao: landscape;
- entrada inicial: teclado no Editor e touch no celular;
- camera: terceira pessoa simples ou primeira pessoa simples;
- cena unica ate a primeira entrega jogavel.

Evitar no inicio:

- mundo aberto;
- multiplayer;
- inventario complexo;
- inimigos com IA avancada;
- graficos realistas;
- assets pesados da Asset Store;
- VR e mobile ao mesmo tempo antes de existir um jogo basico.

### 2. Validar Android na primeira metade do projeto

A validacao Android deve acontecer cedo, mesmo que o jogo ainda tenha apenas:

- um chao;
- um jogador;
- uma camera;
- um objetivo coletavel;
- uma tela de vitoria simples.

Regra pratica: **ate a semana 3 do projeto, cada grupo deve apresentar a primeira evidencia de execucao ou configuracao Android**.

### 3. Trabalhar com MVP jogavel

Em vez de construir varias partes incompletas, cada grupo deve entregar primeiro uma versao minima jogavel:

1. jogador se move;
2. camera acompanha;
3. existe um objetivo;
4. existe uma condicao de vitoria ou derrota;
5. roda no Editor;
6. roda em pelo menos um celular Android do grupo.

Depois disso, o grupo pode melhorar controles, visual, audio, fases e polimento.

### 4. Separar requisitos essenciais e recursos extras

As entregas devem separar o que e obrigatorio para o funcionamento do jogo e o que entra como melhoria de acabamento:

- **obrigatorias:** logica de jogo, cena simples, interacao, build ou video do teste;
- **extras:** shaders, particulas, modelos complexos, efeitos visuais, iluminacao avancada.

Essa separacao ajuda o grupo a priorizar jogabilidade, clareza e validacao tecnica antes do polimento visual.

## Estrutura sugerida de entregas

Cronograma definido em **06/05/2026**, considerando aulas as quintas-feiras. O trabalho deve estar pronto na ultima semana de junho, com entrega final em **25/06/2026**.

| Data | Aula | Marco | Entrega | Evidencia |
|------|------|-------|---------|-----------|
| 07/05/2026 | Aula 1 | Ideia, escopo e ferramentas | Projeto criado, GDD reduzido, padrao tecnico definido, acesso ao Unity Cloud Studio e exploracao do Mixamo | print do Unity + GDD + print das ferramentas |
| 14/05/2026 | Aula 2 | Prototipo de movimento | Cena 3D com jogador, camera, movimento e colisao basica | video curto no Editor |
| 21/05/2026 | Aula 3 | Primeira validacao Android | Primeiro build Android do projeto | APK ou video no celular |
| 28/05/2026 | Aula 4 | Regra principal | Objetivo, pontuacao/progresso e condicao de vitoria | video de gameplay |
| 04/06/2026 | Aula 5 | Desafio | Obstaculos, inimigo simples, timer ou outro elemento de dificuldade | video vencendo e perdendo |
| 11/06/2026 | Aula 6 | Interface e feedback | UI minima, audio e feedback visual | video + prints |
| 18/06/2026 | Aula 7 | Otimizacao mobile | Build atualizado com ajustes de performance | video no celular + checklist de otimizacao |
| 25/06/2026 | Aula 8 | Entrega final | APK final, video de gameplay, GDD atualizado e creditos | pacote final do grupo |

## Organizacao da producao

Durante a trilha, cada grupo deve:

- manter o GDD atualizado;
- definir um responsavel pelo build Android;
- registrar evidencias de execucao a cada marco;
- documentar assets externos utilizados;
- manter o projeto organizado por pastas;
- apresentar progresso por funcionalidades, nao apenas por aparencia visual.

## Metodologia escolhida

A metodologia mais simples para este trabalho e o **MVP jogavel por marcos**:

1. **Ideia curta:** o grupo define um jogo que possa ser explicado em ate 3 frases.
2. **Cena unica:** o projeto comeca com uma fase simples, sem menu complexo.
3. **Jogabilidade primeiro:** movimento, camera, colisao e objetivo aparecem antes do visual final.
4. **Android cedo:** o build mobile e validado antes do projeto crescer.
5. **Incrementos semanais:** cada entrega adiciona uma funcao clara ao jogo.
6. **Polimento no final:** audio, UI, efeitos e materiais entram depois que o jogo ja funciona.

Essa metodologia facilita o acompanhamento do professor e ajuda os grupos a manterem foco em um jogo pequeno, completo e demonstravel.

## Arquivos deste pacote

- [roteiro-alunos.md](roteiro-alunos.md): roteiro que pode ser enviado diretamente aos estudantes.
- [checklist-entrega-mobile.md](checklist-entrega-mobile.md): checklist de entrega e avaliacao.
- [plano-aulas-unity-mobile.md](plano-aulas-unity-mobile.md): sequencia de aulas/labs para conduzir a trilha Unity 3D + Mobile.
- [metodologia-mvp-jogavel.md](metodologia-mvp-jogavel.md): descricao da metodologia de trabalho adotada.
- [roteiro-build-android.md](roteiro-build-android.md): passo a passo completo para gerar, instalar e testar o APK Android.
- [roteiro-unity-cloud-mixamo.md](roteiro-unity-cloud-mixamo.md): roteiro da Aula 1 para Unity Cloud Studio e Mixamo.
