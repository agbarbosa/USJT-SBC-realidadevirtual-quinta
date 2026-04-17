# Aula 01 — Unity na Prática: Interface, GDD em Papel e Primeiros Passos em Casa

**Data:** 16/04/2026 (Quinta-feira)
**Horário:** 19:00 – 21:40
**Disciplina:** Computação Gráfica e Realidade Virtual (0016187)
**Professor:** Alexandre Barbosa

---

## Contexto desta aula

A Aula 00 (09/04) já cobriu: apresentação, alinhamento dos dois projetos do semestre (Cardboard VR + Jogo 2D), escopo da A3, formação inicial de grupos e tarefa de casa (instalar Unity Hub + baixar template do Cardboard).

**Situação atual:**
- Grupos ainda precisam ser formalizados com nomes completos dos integrantes
- Alunos provavelmente NÃO têm Unity instalado (a maioria)
- Nenhum aluno tem computador disponível em sala
- Professor tem projetor disponível

**Estratégia desta aula:** aula expositiva + dinâmica em papel + dever de casa detalhado. Ao sair da aula, cada aluno deve saber exatamente o que fazer em casa e ter um documento de design do jogo (GDD) esboçado no papel.

---

## Agenda

| Horário | Duração | Atividade |
|---------|---------|-----------|
| 19:00 – 19:15 | 15 min | Registro formal dos grupos (formulário impresso) |
| 19:15 – 19:35 | 20 min | O que é Unity? Demo no projetor: Unity Hub e criação de projeto |
| 19:35 – 20:10 | 35 min | Tour pela interface do Unity (demo ao vivo no projetor) |
| 20:10 – 20:20 | 10 min | Conceito de GDD (Game Design Document) |
| 20:20 – 20:30 | 10 min | **Intervalo** |
| 20:30 – 21:10 | 40 min | Dinâmica: grupos preenchem o GDD no papel |
| 21:10 – 21:30 | 20 min | Apresentação rápida dos GDDs (2 min por grupo) |
| 21:30 – 21:40 | 10 min | Roteiro do dever de casa + encerramento |

---

## Bloco 1 — Registro dos Grupos (19:00 – 19:15)

Distribuir o formulário impresso `grupo-registro_2026-04-16.html` (ou projetar na tela e pedir que preencham em papel avulso).

Cada grupo deve informar:
- **Nome do grupo**
- **Nome completo de cada integrante**
- **E-mail do líder do grupo**
- **Ideia inicial do jogo** (gênero + tema, 1–2 frases)
- **Quem vai ser responsável por instalar Unity e testar o build Android**

> Recolher os formulários ao final da aula. Digitalizar ou registrar no arquivo de grupos do semestre.

---

## Bloco 2 — O que é Unity? Demo no Projetor (19:15 – 19:35)

### O que mostrar no projetor

#### 2.1 Contexto: por que Unity para este projeto?

- Motor de jogos mais usado no mundo (mobile, PC, console, VR/AR)
- Gratuito para uso pessoal e acadêmico (licença Personal)
- Exporta para Android com poucas configurações
- Tem suporte nativo ao Google Cardboard XR SDK
- Grande comunidade: tutoriais em português disponíveis

#### 2.2 Unity Hub — o gerenciador de versões

Abrir o site https://unity.com/download e mostrar:
- Página de download do Unity Hub
- Diferença entre Unity Hub (gerenciador) e Unity Editor (o motor em si)
- Qual versão instalar: **Unity 6 LTS** (versão de longo suporte — mais estável)
- Módulos necessários na instalação:
  - `Android Build Support`
  - `Android SDK & NDK Tools`
  - `OpenJDK`
  - `Visual Studio Community` (ou VS Code)

#### 2.3 Criar um novo projeto (demo ao vivo)

Abrir Unity Hub e criar projeto em tempo real:
1. Clicar em **New project**
2. Selecionar template **2D (Built-in Render Pipeline)**
3. Nomear como `MeuJogo2D`
4. Mostrar a tela de carregamento enquanto o projeto abre

---

## Bloco 3 — Tour pela Interface do Unity (19:35 – 20:10)

### Os 5 painéis essenciais

Mostrar cada painel no projetor, explicando o papel de cada um:

| Painel | Localização padrão | Para que serve |
|--------|--------------------|----------------|
| **Scene View** | Centro | Montar a cena visualmente, arrastar objetos |
| **Game View** | Centro (aba ao lado) | Prévia do que o jogador vê; onde você aperta Play |
| **Hierarchy** | Esquerda | Lista todos os objetos da cena (GameObjects) |
| **Inspector** | Direita | Mostra e edita as propriedades do objeto selecionado |
| **Project** | Baixo | Todos os arquivos do projeto (assets, scripts, cenas) |

### O que é um GameObject?

Tudo em Unity é um **GameObject**: a câmera, o personagem, o chão, o inimigo, a luz.
Cada GameObject pode ter **Componentes** que definem seu comportamento:

| Componente | O que faz |
|------------|-----------|
| `Transform` | Posição, rotação e escala no mundo |
| `Sprite Renderer` | Exibe uma imagem 2D |
| `Rigidbody 2D` | Aplica física (gravidade, colisões) |
| `Collider 2D` | Define a forma de colisão |
| `Script (C#)` | Comportamento personalizado |

### Demo ao vivo: criar um objeto simples

1. **Hierarchy → clique direito → 2D Object → Sprite → Square**
2. Renomear para `Jogador`
3. No **Inspector**: mudar a cor no Sprite Renderer
4. Mostrar o **Transform**: mudar posição X, Y e ver o objeto se mover na Scene View
5. Adicionar **Rigidbody 2D**: o quadrado cai por gravidade ao apertar Play

> Este é o ciclo básico de trabalho em Unity: criar GameObject → adicionar componentes → apertar Play → observar comportamento → ajustar.

---

## Bloco 4 — O que é um GDD? (20:10 – 20:20)

### Game Design Document (Documento de Design de Jogo)

O GDD é o **documento de referência do grupo** — o "contrato" sobre o que o jogo vai ser. Usado na indústria antes de escrever uma linha de código.

**Por que fazer antes de codificar?**
- Alinha todos do grupo em torno de uma mesma visão
- Evita retrabalho e conflitos sobre decisões de design
- Facilita dividir o trabalho entre os membros
- Serve como guia durante o desenvolvimento

### Estrutura mínima do GDD para este projeto

| Seção | Descrição |
|-------|-----------|
| **Título e conceito** | Nome do jogo + 1 parágrafo de pitch |
| **Gênero** | Plataforma, runner, shooter, puzzle... |
| **Mecânica principal** | A ação central do jogador (ex: "pular entre plataformas") |
| **Personagem principal** | Quem é, o que pode fazer, como se parece |
| **Cenário** | Onde se passa o jogo (floresta, espaço, cidade...) |
| **Obstáculos/inimigos** | O que dificulta a vida do jogador |
| **Sistema de pontuação** | Como o jogador ganha/perde pontos |
| **Esboço da tela principal** | Desenho (mesmo que tosco) do layout do jogo |

---

## Bloco 5 — Dinâmica: GDD em Papel (20:30 – 21:10)

### Instruções para os grupos

Cada grupo recebe uma folha de papel (ou usa o verso do formulário de registro) e preenche o GDD mínimo.

**Tempo:** 30 min para preencher + 10 min para apresentar.

**O que cada grupo deve entregar ao final:**
- [ ] Título do jogo
- [ ] Gênero escolhido
- [ ] Descrição da mecânica principal (1 parágrafo)
- [ ] Esboço desenhado à mão da tela principal do jogo
- [ ] Divisão inicial de responsabilidades no grupo

> O professor circula pela sala durante os 30 min para tirar dúvidas, estimular decisões e ajudar grupos travados.

### Sugestões de mecânicas simples (para grupos sem ideia)

| Gênero | Mecânica central | Complexidade |
|--------|-----------------|--------------|
| Endless runner | Personagem corre, jogador pula obstáculos | ⭐ |
| Plataforma | Mover + pular entre plataformas | ⭐⭐ |
| Shooter simples | Nave/personagem atira em inimigos | ⭐⭐ |
| Coleta | Personagem coleta itens, evita obstáculos | ⭐ |
| Puzzle de blocos | Empurrar blocos para resolver enigmas | ⭐⭐⭐ |

---

## Bloco 6 — Apresentação dos GDDs (21:10 – 21:30)

Cada grupo tem **2 minutos** para apresentar:
1. Nome do grupo e dos integrantes
2. Título e gênero do jogo
3. A mecânica principal
4. Mostrar o esboço desenhado

> O professor faz anotações sobre cada grupo para referência futura. Recolher as folhas ao final.

---

## Bloco 7 — Roteiro do Dever de Casa (21:30 – 21:40)

Projetar e ler junto com a turma o roteiro detalhado de instalação e primeiros passos (ver arquivo de tarefa abaixo).

**Prazo:** trazer Unity instalado e funcionando na **Aula 02 (23/04)**. Quem não conseguir instalar deve entrar em contato com o professor antes da próxima aula.

---

## Dever de Casa — Roteiro Completo

### Passo 1 — Instalar o Unity Hub

1. Acesse: https://unity.com/download
2. Clique em **Download Unity Hub**
3. Instale normalmente (próximo → próximo → instalar)
4. Abra o Unity Hub e crie uma conta gratuita em unity.com (se não tiver)

### Passo 2 — Instalar o Unity Editor (versão LTS)

1. No Unity Hub, clique em **Installs → Install Editor**
2. Selecione a versão mais recente com o selo **LTS** (Long Term Support)
3. Na tela de módulos, marque:
   - ✅ `Android Build Support`
   - ✅ `Android SDK & NDK Tools`
   - ✅ `OpenJDK`
   - ✅ `Visual Studio Community 2022` (ou VS Code, se preferir)
4. Clique em **Install** — aguardar (pode demorar 30–60 min dependendo da internet)

### Passo 3 — Criar o primeiro projeto

1. No Unity Hub: **New project**
2. Template: **2D (Built-in Render Pipeline)**
3. Nome: `[NomeDoGrupo]_Jogo2D` (ex: `GrupoAlpha_Jogo2D`)
4. Salvar em uma pasta fácil de encontrar (ex: `Documentos/Unity/`)
5. Clicar em **Create project** e aguardar abrir

### Passo 4 — Explorar a interface (15 min)

Com o projeto aberto:
1. Identifique os 5 painéis: Scene, Game, Hierarchy, Inspector, Project
2. **Hierarchy → clique direito → 2D Object → Sprite → Square** — crie um quadrado
3. Renomeie para `Jogador` (clique duplo no nome na Hierarchy)
4. No Inspector, mude a cor do Sprite Renderer (campo Color)
5. Mude os valores de X e Y no Transform e veja o objeto se mover
6. Adicione **Rigidbody 2D**: no Inspector → **Add Component** → buscar "Rigidbody 2D"
7. Aperte **Play** (▶) e observe o objeto cair

### Passo 5 — Habilitar o Modo Desenvolvedor no celular Android

Para a próxima aula podermos testar o jogo direto no celular:
1. Configurações → Sobre o celular → toque **7 vezes** em "Número de compilação"
2. Volte em Configurações → Opções do desenvolvedor → ative **Depuração USB**
3. Conecte o celular ao PC com cabo USB e autorize a depuração quando aparecer o pop-up

### Checklist para trazer na Aula 02 (23/04)

- [ ] Unity Hub instalado
- [ ] Unity LTS instalado com módulos Android
- [ ] Projeto `[NomeDoGrupo]_Jogo2D` criado
- [ ] Já explorou a interface (criou pelo menos 1 objeto)
- [ ] GDD do grupo escrito (pode ser no papel ou digital)
- [ ] Celular com Modo Desenvolvedor ativado
- [ ] Cabo USB data disponível (não só de carga)

---

## Anotações da Aula

_(preencher após a aula)_

- Número de alunos presentes:
- Grupos registrados (quantidade):
- Grupos com Unity já instalado:
- Grupos sem ideia de jogo ainda (precisam de suporte):
- Pendências identificadas:
- Observações gerais:

---

## Próxima Aula — 23/04/2026 (Aula 02)

**Tema:** Primeiro script C# — fazendo o personagem se mover

- Verificar instalação do Unity de cada grupo
- Criar um script de movimento básico (Transform, Input, Time.deltaTime)
- Conceito de Update() vs Start()
- Conectar o movimento do personagem às teclas do teclado
- Importar um sprite (imagem) para o personagem
