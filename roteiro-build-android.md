# Roteiro Completo: Gerar a Versao Android do Jogo no Unity

## Objetivo

Este roteiro orienta o grupo a configurar o projeto Unity e gerar uma versao Android do jogo em formato `.apk`.

Ao final, o grupo deve conseguir:

- configurar o Unity para Android;
- preparar o projeto para build;
- gerar um arquivo `.apk`;
- instalar ou executar o jogo em um celular Android;
- registrar evidencias do teste.

## Padrao da disciplina

Todos os grupos devem usar:

- Unity LTS indicada pelo professor;
- template `3D (Built-in Render Pipeline)`;
- pipeline `Built-in Render Pipeline`;
- plataforma alvo Android;
- cena principal chamada `MainScene`;
- projeto organizado em pastas.

## Parte 1: Conferir se o Unity tem suporte Android

Antes de abrir o projeto, confira se o Unity foi instalado com os modulos corretos.

1. Abra o **Unity Hub**.
2. Clique em **Installs**.
3. Localize a versao do Unity usada no projeto.
4. Clique no icone de engrenagem ou tres pontos.
5. Escolha **Add modules**.
6. Verifique se estes itens estao instalados:
   - `Android Build Support`;
   - `Android SDK & NDK Tools`;
   - `OpenJDK`.

Se algum item nao estiver instalado, marque e instale.

## Parte 2: Preparar o projeto Unity

Abra o projeto do grupo no Unity.

Antes do build, confira:

- o jogo roda ao clicar em **Play**;
- a cena principal esta salva;
- nao ha erros vermelhos no Console;
- o jogador consegue se mover;
- existe uma camera funcional;
- existe pelo menos uma regra de jogo testavel.

Para salvar a cena:

1. Abra a cena principal.
2. Va em **File > Save**.
3. Confirme que a cena esta em `Assets/Scenes/MainScene`.

## Parte 3: Adicionar a cena no Build Settings

O Unity so inclui no APK as cenas listadas no Build Settings.

1. Va em **File > Build Settings**.
2. Na parte superior, localize **Scenes In Build**.
3. Clique em **Add Open Scenes**.
4. Confirme que `MainScene` apareceu na lista.

Se houver mais de uma cena, deixe a cena inicial no topo da lista.

## Parte 4: Trocar a plataforma para Android

1. Ainda em **File > Build Settings**.
2. Na lista de plataformas, selecione **Android**.
3. Clique em **Switch Platform**.
4. Aguarde o Unity reimportar os arquivos.

Esse processo pode demorar alguns minutos.

Quando terminar, o simbolo do Unity deve aparecer ao lado de **Android**, indicando que Android e a plataforma ativa.

## Parte 5: Configurar Player Settings

No Build Settings, clique em **Player Settings**.

### Company Name

Use um nome simples:

```text
USJT
```

### Product Name

Use o nome do jogo:

```text
NomeDoJogo
```

Evite caracteres especiais no nome do produto.

### Package Name

O Package Name identifica o aplicativo no Android.

Formato recomendado:

```text
com.usjt.nomedogrupo.nomedojogo
```

Exemplo:

```text
com.usjt.grupoalpha.labescape
```

Regras:

- usar apenas letras minusculas;
- nao usar acentos;
- nao usar espacos;
- nao comecar partes com numero;
- separar partes com ponto.

### Version

Use:

```text
1.0
```

### Bundle Version Code

Use:

```text
1
```

Se gerar uma nova versao, pode aumentar para `2`, `3` e assim por diante.

## Parte 6: Configurar orientacao da tela

Em **Player Settings > Resolution and Presentation**:

1. Localize **Default Orientation**.
2. Escolha uma orientacao para o jogo:
   - `Landscape Left`, para jogo deitado;
   - `Portrait`, para jogo em pe.

Para esta disciplina, a recomendacao inicial e:

```text
Landscape Left
```

Use a mesma orientacao durante todo o projeto.

## Parte 7: Configurar qualidade grafica inicial

Para a primeira versao Android, use configuracoes simples.

Em **Edit > Project Settings > Quality**:

1. Localize a coluna do Android.
2. Selecione uma qualidade intermediaria ou baixa.
3. Evite usar qualidade maxima no primeiro build.

Recomendacoes:

- reduzir sombras quando possivel;
- evitar muitas luzes dinamicas;
- evitar excesso de particulas;
- usar materiais simples;
- manter a primeira cena pequena.

## Parte 8: Configurar controles mobile

Antes de gerar o APK final, o jogo precisa funcionar sem teclado.

Opcoes simples para os grupos:

- joystick virtual na tela;
- botoes UI para mover e pular;
- toque na tela para acao principal;
- movimento automatico com botoes para esquerda/direita;
- camera fixa com controles simples.

Para o primeiro build Android, o grupo pode validar apenas:

- a cena abre;
- o jogador aparece;
- a camera funciona;
- pelo menos uma interacao pode ser testada.

Depois, o grupo melhora os controles mobile nos proximos marcos.

## Parte 9: Preparar o celular Android

No celular Android:

1. Abra **Configuracoes**.
2. Entre em **Sobre o telefone**.
3. Toque 7 vezes em **Numero da versao** ou **Numero de compilacao**.
4. Volte para as configuracoes.
5. Abra **Opcoes do desenvolvedor**.
6. Ative **Depuracao USB**.

Ao conectar o celular ao computador:

1. use um cabo USB que transfira dados;
2. desbloqueie a tela do celular;
3. aceite a autorizacao de depuracao USB;
4. mantenha o celular conectado durante o build.

Observacao: alguns cabos USB servem apenas para carregar e nao transferem dados.

## Parte 10: Gerar o APK

No Unity:

1. Va em **File > Build Settings**.
2. Confirme que a plataforma ativa e **Android**.
3. Confirme que `MainScene` esta em **Scenes In Build**.
4. Desmarque **Build App Bundle (Google Play)**, se essa opcao aparecer.
5. Clique em **Build**.
6. Escolha uma pasta para salvar o APK.
7. Use um nome simples:

```text
NomeDoJogo_Android_v1.apk
```

Exemplo:

```text
LabEscape_Android_v1.apk
```

8. Aguarde o Unity finalizar o processo.

Se o build der certo, o Unity vai gerar um arquivo `.apk`.

## Parte 11: Build and Run

Se o celular estiver conectado e autorizado, o grupo tambem pode usar:

```text
Build And Run
```

Esse comando:

1. gera o APK;
2. instala no celular;
3. abre o jogo automaticamente.

Use **Build And Run** para teste rapido. Use **Build** quando precisar entregar o arquivo APK.

## Parte 12: Instalar o APK manualmente

Se o grupo gerou o APK mas nao usou Build And Run:

1. envie o APK para o celular;
2. abra o arquivo no celular;
3. autorize a instalacao de apps dessa fonte;
4. instale o jogo;
5. abra o aplicativo.

O Android pode exibir um aviso de seguranca porque o APK nao veio da Play Store. Para este trabalho, isso e esperado em builds de teste.

## Parte 13: Testar no celular

Depois de abrir o jogo no Android, testar:

- o jogo abre sem fechar sozinho;
- a cena correta aparece;
- a camera mostra o jogador ou o ambiente corretamente;
- os controles funcionam;
- a interface aparece no tamanho correto;
- textos nao ficam cortados;
- a condicao de vitoria ou objetivo funciona;
- o jogo nao trava durante o teste.

Grave um video curto de 30 a 60 segundos mostrando:

1. o icone ou abertura do jogo;
2. a cena principal;
3. movimento ou interacao;
4. objetivo ou pontuacao;
5. fim, vitoria ou estado jogavel.

## Parte 14: O que entregar

Para a entrega Android, o grupo deve enviar:

- arquivo `.apk`;
- video curto do jogo rodando no celular;
- print do Build Settings;
- versao do Unity usada;
- nome do responsavel pelo build Android.

Modelo de registro:

```text
Grupo:
Nome do jogo:
Versao Unity:
Template: 3D (Built-in Render Pipeline)
Pipeline: Built-in Render Pipeline
Nome do APK:
Celular usado no teste:
Responsavel pelo build:
Data do build:
Observacoes:
```

## Parte 15: Erros comuns e solucoes

### Android nao aparece como plataforma

Causa provavel: modulo Android nao instalado.

Solucao:

1. abrir Unity Hub;
2. ir em **Installs**;
3. clicar em **Add modules**;
4. instalar `Android Build Support`, `Android SDK & NDK Tools` e `OpenJDK`.

### Erro de SDK, NDK ou JDK

Causa provavel: ferramentas Android ausentes ou configuracao incorreta.

Solucao:

1. conferir os modulos Android no Unity Hub;
2. abrir **Edit > Preferences > External Tools**;
3. verificar se Unity esta usando as ferramentas instaladas com o Editor;
4. fechar e abrir o Unity novamente.

### Cena errada abre no celular

Causa provavel: cena principal nao esta no Build Settings ou nao esta no topo.

Solucao:

1. abrir `MainScene`;
2. ir em **File > Build Settings**;
3. clicar em **Add Open Scenes**;
4. deixar `MainScene` como primeira cena da lista.

### Jogo abre com tela preta

Possiveis causas:

- camera nao esta ativa;
- camera esta virada para o lado errado;
- jogador esta fora do campo de visao;
- cena errada foi adicionada no build;
- luzes ou objetos foram removidos.

Solucao:

1. testar a cena no Editor;
2. conferir se existe uma camera ativa;
3. conferir a posicao da camera;
4. conferir se `MainScene` esta no Build Settings;
5. gerar o APK novamente.

### Controles funcionam no computador, mas nao no celular

Causa provavel: o jogo depende de teclado ou mouse.

Solucao:

1. adicionar botoes na tela;
2. adicionar joystick virtual;
3. usar toque na tela para a acao principal;
4. testar novamente no Android.

### APK instala, mas fecha sozinho

Possiveis causas:

- erro de script;
- cena muito pesada;
- celular sem memoria suficiente;
- objeto importante nao foi incluido;
- configuracao Android incorreta.

Solucao:

1. verificar erros no Console do Unity;
2. reduzir elementos pesados da cena;
3. testar em uma cena mais simples;
4. gerar novo build;
5. registrar o erro para analise.

### Interface fica cortada

Causa provavel: Canvas sem configuracao responsiva.

Solucao:

1. selecionar o Canvas;
2. no componente **Canvas Scaler**, usar `Scale With Screen Size`;
3. definir uma resolucao de referencia, como `1920 x 1080`;
4. testar novamente em landscape.

### Build demora muito

Isso pode acontecer no primeiro build.

Recomendacoes:

- fechar programas pesados;
- salvar o projeto antes do build;
- evitar assets muito grandes;
- fazer build de uma cena simples primeiro;
- aguardar o Unity terminar sem fechar o programa.

## Checklist rapido antes de clicar em Build

- [ ] Projeto abre sem erros vermelhos.
- [ ] `MainScene` esta salva.
- [ ] `MainScene` esta em **Scenes In Build**.
- [ ] Plataforma ativa e Android.
- [ ] Package Name esta preenchido corretamente.
- [ ] Orientacao da tela foi definida.
- [ ] Controles mobile foram planejados ou implementados.
- [ ] Cena foi testada no Editor.
- [ ] APK sera salvo com nome claro.

## Checklist rapido depois do build

- [ ] APK foi gerado.
- [ ] APK foi instalado ou executado no celular.
- [ ] Jogo abriu no Android.
- [ ] Cena correta apareceu.
- [ ] Controle ou interacao principal funcionou.
- [ ] Video de evidencia foi gravado.
- [ ] Arquivo foi separado para entrega.

