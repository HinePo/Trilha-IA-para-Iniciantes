# Trilha AI Quick Start para iniciantes

Uma trilha prática para quem ficou de fora dos avanços recentes em Inteligência Artificial e quer começar sem complicação.

> Esta trilha foi feita para iniciantes de qualquer idade. Ela apresenta as ideias e ferramentas mais importantes, mas não é uma formação aprofundada nem avançada. O objetivo é começar a usar IA com segurança, criar pequenos projetos e aprender o restante conforme a necessidade.

> Alguns links desta trilha levam a páginas em inglês. Se precisar, clique com o botão direito na página e escolha **Traduzir para Português** (disponível na maioria dos navegadores, como Chrome e Edge).

> Se ficar alguma dúvida em qualquer ponto da trilha, pergunte para uma IA. Não é necessário entender tudo a fundo antes de continuar: entenda o suficiente para seguir em frente e volte ao assunto depois, se precisar.


## Objetivos da trilha

Ao final, a pessoa deverá conseguir:

- conversar com uma IA de forma clara e melhorar seus próprios prompts;
- entender, em linguagem simples, o que são LLMs, contexto, alucinação, tools, skills e Agents;
- usar IA para estudar, pesquisar, escrever, analisar dados e criar arquivos;
- experimentar uma arquitetura simples com um coordinator e workers especializados;
- abrir e modificar um notebook no Google Colab;
- organizar um projeto em pastas fáceis de entender por pessoas e Agents;
- usar um Agent dentro do VS Code ou do Cursor para criar e testar um projeto pequeno;
- entender para que servem Git, GitHub, testes e documentação;
- saber conferir o trabalho da IA em vez de aceitar tudo automaticamente.

## Como estudar

Esta não é uma lista de cursos obrigatórios. A melhor sequência é **experimentar, assistir somente ao vídeo necessário e voltar para a prática**.

| Ritmo | Recomendação |
|---|---|
| Duração total | 8 a 12 semanas, sem pressa |
| Frequência | 2 encontros por semana |
| Cada encontro | 45 a 75 minutos |
| Divisão do tempo | Cerca de 15 minutos de conteúdo e o restante de prática |
| Regra principal | Sempre terminar com algo criado, modificado ou testado |
| <span style="color: orange"><strong>Quando travar</strong></span> | <span style="color: orange"><strong>Pedir uma explicação simples à IA e continuar em passos menores</strong></span> |

## Mapa rápido da trilha

| Etapa | Tema | Resultado prático | Tempo sugerido |
|---|---|---|---|
| 1 | Primeiro contato com IA | Criar, comparar e melhorar respostas | 1 semana |
| 2 | Conceitos fundamentais | Entender prompts, LLMs, contexto, erros e verificação | 1 semana |
| 3 | Grok Bot e Agents | Criar três Bots especializados e experimentar um chat em grupo | 1 a 2 semanas |
| 4 | Colab e Python básico | Executar e modificar pequenos códigos | 2 semanas |
| 5 | Projeto bem organizado | Montar pastas, documentação e README | 1 semana |
| 6 | Agents para código | Usar Claude Code, Codex ou Cursor em um projeto | 2 a 3 semanas |
| 7 | Qualidade | Pedir testes, revisão e correções | 1 semana |
| Bônus | Git e GitHub | Criar versões e compartilhar o projeto | 1 a 2 semanas |

## 1. Primeiro contato com Inteligência Artificial

Comece usando uma IA pela web. Não é necessário instalar nada.

| Plataforma | Link | Para começar |
|---|---|---|
| ChatGPT | [Abrir ChatGPT](https://chatgpt.com/) | Conversar, pesquisar, trabalhar com arquivos e criar conteúdo |
| Gemini | [Abrir Gemini](https://gemini.google.com/) | Conversar e trabalhar com ferramentas do Google |
| Claude | [Abrir Claude](https://claude.ai/) | Conversar, analisar documentos e criar conteúdo |
| Grok | [Abrir Grok](https://grok.com/) | Conversar, pesquisar e criar mídia |

Os planos gratuitos, limites e recursos mudam com frequência. Para iniciar, escolha **uma** plataforma disponível e use a mesma durante alguns dias. Depois compare com outra.

### Três experiências de 15 minutos

| Experiência | Prompt inicial | O que observar |
|---|---|---|
| Aprender | `Explique fotossíntese para um iniciante, com um exemplo e cinco perguntas de revisão.` | A explicação ficou clara? As perguntas ajudam? |
| Criar | `Crie um quiz de dez perguntas sobre Pokémon. Mostre uma pergunta por vez e espere minha resposta.` | A IA segue o formato pedido? |
| Planejar | `Ajude-me a dividir um trabalho escolar sobre o Sistema Solar em pequenas tarefas para cinco dias.` | O plano é realista? Falta alguma etapa? |

Depois de cada resposta, peça uma melhoria: mais curto, mais simples, em tabela, com exemplos, com fontes ou com perguntas antes de responder.

## 2. Conceitos principais sem complicação

| Conceito | Explicação simples | Exemplo |
|---|---|---|
| Inteligência Artificial | Sistemas capazes de realizar tarefas que normalmente exigem decisões humanas | Reconhecer uma imagem ou responder a uma pergunta |
| IA generativa | IA que cria conteúdo novo | Texto, imagem, áudio, vídeo, planilha ou código |
| LLM | Modelo treinado com muitos textos para trabalhar com linguagem | O modelo que produz a resposta de um chat |
| Prompt | O pedido enviado para a IA | `Explique este texto em cinco tópicos` |
| Contexto | As informações disponíveis para a IA naquele momento | Conversa, arquivos, regras e trechos do projeto |
| Token | Pequeno pedaço de texto processado pelo modelo | Uma palavra pode ser dividida em mais de um token |
| Alucinação | Resposta inventada ou incorreta apresentada de forma convincente | Uma fonte ou número que não existe |
| Tool | Uma ferramenta que permite ao Agent fazer uma ação | Ler arquivo, buscar na web ou executar um comando |
| Agent | IA que recebe um objetivo, escolhe passos e usa tools para trabalhar | Ler os arquivos, editar o projeto e executar testes |
| Subagent | Um Agent invocado (ou criado) por outro Agent para cuidar de uma parte específica da tarefa | Um Agent principal chama um subagent apenas para rodar e revisar os testes |
| Skill | Instrução reutilizável para uma tarefa específica | Como revisar um texto ou montar uma apresentação |
| Rule | Regra que orienta o comportamento do Agent | `Sempre execute os testes antes de concluir` |
| RAG | Forma de responder consultando materiais externos relevantes | Buscar a resposta nos PDFs de uma disciplina |

### Um modelo simples de bom prompt

Use esta estrutura sem tentar decorar nomes técnicos:

```text
Objetivo: o que eu quero produzir?
Contexto: quais informações a IA precisa saber?
Formato: como a resposta deve ser organizada?
Critérios: o que precisa ser conferido ou respeitado?
```

No item Contexto, sempre que possível, **anexe os arquivos relevantes** (PDF, planilha, imagem, trecho de código) em vez de só descrever o conteúdo de memória. Isso reduz alucinação e deixa a resposta mais precisa.

Exemplo:

```text
Quero revisar para uma prova de História.
Use somente o PDF anexado e explique o capítulo 3 para um iniciante.
Organize em uma tabela com tema, explicação e exemplo.
Depois crie cinco perguntas, uma por vez.
Se uma informação não estiver no PDF, avise em vez de inventar.
```

### Há muitas ferramentas, mas a lógica está convergindo

Os nomes e as telas mudam, mas as plataformas modernas estão ficando parecidas. Em quase todas elas, o usuário descreve um objetivo e o sistema combina contexto, planejamento, tools e verificação.

| Capacidade comum | Chat de IA | Agent de código | Grok Bot |
|---|---:|---:|---:|
| Conversar em linguagem natural | Sim | Sim | Sim |
| Ler arquivos e instruções | Sim | Sim | Sim |
| Planejar uma tarefa | Sim | Sim | Sim |
| Usar ferramentas | Algumas | Muitas | Muitas |
| Editar arquivos | Depende da plataforma | Sim | Sim, no computador do Bot |
| Executar tarefas em várias etapas | Depende do modo | Sim | Sim |
| Trabalhar com Agents especializados | Em algumas plataformas | Sim | Sim |
| Pedir aprovação antes de ações importantes | Em algumas plataformas | Sim | Sim |

O aprendizado mais durável não é decorar cada botão. É saber explicar o objetivo, fornecer o contexto certo, dividir o trabalho, revisar o plano e conferir o resultado.

## 3. Agents e arquitetura multi-agent

Um Agent não é apenas um chat que responde. Ele pode receber um objetivo, examinar arquivos, escolher ações, usar tools, criar ou delegar tarefas e verificar o resultado.

### Modelo mental: coordinator e workers

| Papel | Responsabilidade | Exemplo |
|---|---|---|
| Coordinator | Recebe o pedido principal, cria o plano, distribui tarefas e reúne os resultados | Coordenar um trabalho escolar completo |
| Worker de pesquisa | Procura e resume fontes | Encontrar informações e guardar links |
| Worker de escrita | Produz ou revisa o texto | Transformar notas em um relatório |
| Worker de dados | Trabalha com tabelas e gráficos | Analisar uma planilha |
| Worker de qualidade | Confere requisitos, erros e testes | Revisar o resultado antes da entrega |

A ideia é enviar os pedidos principalmente ao **coordinator**. Ele pode usar workers existentes ou criar novos quando necessário. Cada worker pode ter:

- um papel e uma descrição;
- instruções próprias;
- skills específicas;
- tools permitidas ou proibidas;
- limites de acesso;
- um formato de resposta esperado.

No começo, use poucos Agents. Um coordinator e dois ou três workers já demonstram toda a lógica.

## 4. Grok Bot: primeira experiência com vários Agents

O [Grok Bot](https://x.ai/bot) permite criar Bots persistentes, dar um papel para cada um e colocá-los para colaborar. Os Bots compartilham um computador em nuvem, mas mantêm conversas e papéis próprios. O acesso depende de um plano compatível.

> Para quem nunca trabalhou com Agents, o Grok Bot pode ser o **melhor ponto de partida** da trilha. Ele é simples de configurar, roda no navegador sem instalar nada, e mostra de forma visual cada Bot, seu papel e a troca de mensagens entre eles. Isso ajuda a construir o modelo mental de coordinator e workers antes de lidar com Agents de código, que são mais poderosos, mas também mais abstratos.

<span style="color: orange"><strong>A ideia central é criar um time de Agents, como na vida real: cada Bot tem uma função, instruções e habilidades diferentes, do mesmo jeito que um grupo de trabalho na escola, faculdade ou empresa costuma dividir tarefas entre pessoas diferentes.</strong></span> Você pode conversar com cada Bot individualmente ou colocar todos em um **group chat**, como um grupo de WhatsApp de trabalho, onde eles colaboram entre si e com você para chegar ao resultado.

Links úteis:

- [Visão geral do Grok Bot](https://docs.x.ai/grok-bot/overview)
- [Primeiros passos](https://docs.x.ai/grok-bot/get-started)
- [Criar e gerenciar Bots](https://docs.x.ai/grok-bot/bots)
- [Chat e colaboração](https://docs.x.ai/grok-bot/chat-and-collaboration)
- [Skills, rotinas e automações](https://docs.x.ai/grok-bot/skills-routines-and-automations)
- [Download do Grok Bot](https://cursor.com/download/bot)

### Três Bots para criar

| Bot | Papel sugerido | Primeira tarefa |
|---|---|---|
| Coordenador | Conversar com o usuário, dividir tarefas e chamar os outros Bots | Organizar um projeto sobre um tema escolhido |
| Pesquisador | Buscar informações, registrar fontes e apontar dúvidas | Criar uma lista curta de fontes confiáveis |
| Produtor | Criar documentos, tabelas, apresentações e revisar o acabamento | Transformar a pesquisa em materiais de entrega |

Não é necessário programar nada para criar cada Bot. <span style="color: orange"><strong>Basta instruir, falando ou escrevendo, explicando para o Agent o que você quer criar: o papel do Bot</strong></span>, como ele deve se comportar e qual é sua primeira tarefa.

### Exercício em chat de grupo

1. Crie os três Bots.
2. Abra uma conversa com o Coordenador.
3. Adicione os outros Bots ao mesmo grupo.
4. Envie somente ao Coordenador:

```text
Coordene os outros Bots para criar um pequeno kit sobre energia solar.
Quero:
1. um documento Word de duas páginas;
2. uma planilha Excel com dez exemplos e três colunas;
3. uma apresentação de cinco slides.
Antes de começar, mostre a divisão de tarefas. No final, revise se todos os arquivos estão claros e consistentes.
```

Depois, repita com um tema de interesse pessoal. As ações disponíveis dependem dos aplicativos conectados, dos logins e das permissões concedidas. Revise qualquer ação externa antes de aprovar.

## 5. Google Colab e Python básico

O [Google Colab](https://colab.research.google.com/?hl=pt_BR) permite executar Python no navegador usando notebooks. Para esta etapa, não é necessário instalar Python no computador.

Links para começar:

- [Abrir o Google Colab](https://colab.research.google.com/?hl=pt_BR)
- [Notebook introdutório oficial](https://colab.research.google.com/notebooks/intro.ipynb?hl=pt_BR)
- [Curso Básico de Python da Hashtag Programação](https://www.youtube.com/playlist?list=PLpdAy0tYrnKwgyv8Rc867jA_huQfcpF29)
- [Python 3 Mundo 1 do Curso em Vídeo](https://www.youtube.com/playlist?list=PLHz_AreHm4dlKP6QQCekuIPky1CiwmdI6)

### Como usar o Colab

1. Abra o Colab e entre com uma conta Google.
2. Clique em **Novo notebook**.
3. Escreva código em uma célula.
4. Clique no botão de executar ou use `Shift + Enter`.
5. Leia a saída logo abaixo.
6. Renomeie o notebook e confirme que ele foi salvo no Google Drive.

Primeira célula:

```python
nome = "Pikachu"
ataque = 55
defesa = 40

print(nome)
print(ataque > defesa)
```

Altere os valores, tente prever a saída e execute novamente.

### O mínimo de Python para começar

| Tema | O que precisa entender | Exercício curto |
|---|---|---|
| Variáveis | Guardam valores com nomes | Nome, ataque e defesa de um personagem |
| Tipos | Texto, inteiro, decimal e verdadeiro/falso | Conferir o tipo de três valores |
| Listas | Guardam vários itens em ordem | Criar uma equipe com cinco personagens |
| `if` e `else` | Escolhem uma ação conforme uma condição | Informar quem venceu uma batalha |
| `for` | Repete uma ação para cada item | Mostrar todos os nomes da equipe |
| Funções | Reúnem passos que podem ser reutilizados | Criar `calcular_pontos()` |

<span style="color: orange"><strong>Não é necessário dominar tudo antes de criar. Peça à IA para criar o código, explicar o código, faça uma alteração pequena, execute e confira.</strong></span>

### Exercícios clássicos com funções

Bons primeiros exercícios para fixar funções, `if`/`else` e `for` na prática, testando a mesma função com vários casos diferentes.

**Calculadora de IMC**

Crie uma função que recebe peso (kg) e altura (m), calcula o IMC (`peso / altura²`) e informa se o valor está entre 25 e 30 (sobrepeso, segundo a OMS).

```python
def calcular_imc(peso, altura):
    imc = peso / altura ** 2
    sobrepeso = 25 <= imc < 30
    return round(imc, 1), sobrepeso

pessoas = [
    ("Pessoa 1", 68, 1.70),
    ("Pessoa 2", 90, 1.75),
    ("Pessoa 3", 55, 1.60),
]

for nome, peso, altura in pessoas:
    imc, sobrepeso = calcular_imc(peso, altura)
    print(nome, imc, "sobrepeso" if sobrepeso else "fora da faixa")
```

Peça à IA para explicar cada linha, depois peça para adicionar outras faixas (abaixo do peso, peso normal, obesidade).

**Outras ideias no mesmo formato**

- **Conversor de temperatura:** uma função `celsius_para_fahrenheit(c)` aplicada a uma lista de temperaturas, mostrando quais ultrapassam 30°C.
- **Verificador de palíndromo:** uma função `eh_palindromo(palavra)` testada com uma lista de palavras (ex.: `"arara"`, `"colab"`, `"ovo"`), ignorando maiúsculas e espaços.

O padrão se repete: escrever a função, montar uma lista de casos de teste e usar `for` para aplicar a função a todos eles de uma vez.

### Projeto rápido com dados de Pokémon

Use o notebook [Learn Pandas with Pokémons](https://www.kaggle.com/code/ash316/learn-pandas-with-pokemons) apenas como inspiração. Para o primeiro projeto, use poucas colunas: nome, tipo, ataque, defesa e velocidade.

Perguntas possíveis:

- Quais são os cinco Pokémon mais rápidos?
- Qual tipo tem maior ataque médio?
- Entre os Pokémon de água, quais têm defesa acima de 70?
- Qual gráfico ajuda a comparar ataque e defesa?

Peça à IA para produzir um passo de cada vez e explicar cada nova linha. Sempre confira algumas linhas manualmente.

## 6. Vídeos e playlists em português brasileiro

Use os vídeos sob demanda. Não é necessário terminar todas as playlists.

| Tema | Material | Como usar |
|---|---|---|
| Visão geral de IA | [Canal Hashtag Treinamentos](https://www.youtube.com/@HashtagTreinamentos) | Buscar vídeos introdutórios sobre IA, ChatGPT e prompts |
| IA generativa | [Curso em Vídeo — Inteligência Artificial, módulo 1](https://www.youtube.com/playlist?list=PLHz_AreHm4dm24MhlWJYiR_Rm7TFtvs6S) | Selecionar as aulas sobre IA, LLMs, prompts e alucinações |
| IA para estudar e criar | [Curso em Vídeo — Inteligência Artificial, módulo 2](https://www.youtube.com/playlist?list=PLHz_AreHm4dk0Hg99bUQMiH1dEn-qu0Hg) | Assistir depois das primeiras práticas |
| Prompt na prática | [Engenharia de Prompt — Hashtag](https://www.hashtagtreinamentos.com/engenharia-de-prompt-ia) | Ler o resumo e testar as ideias imediatamente |
| Python curto | [Curso Básico de Python — Hashtag](https://www.youtube.com/playlist?list=PLpdAy0tYrnKwgyv8Rc867jA_huQfcpF29) | Priorizar variáveis, strings, listas, `if` e `for` |
| Python com mais exercícios | [Python 3 Mundo 1 — Curso em Vídeo](https://www.youtube.com/playlist?list=PLHz_AreHm4dlKP6QQCekuIPky1CiwmdI6) | Consultar somente quando precisar reforçar um fundamento |

## 7. Estrutura de projeto simples e agent-friendly

Um Agent trabalha melhor quando encontra nomes claros, documentação curta e arquivos no lugar esperado.

Estrutura recomendada:

```text
meu-projeto/
├── README.md
├── AGENTS.md ou CLAUDE.md
├── docs/
│   ├── fontes/
│   ├── imagens/
│   └── requisitos.md
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
├── src/
├── tests/
├── outputs/
├── pyproject.toml
└── .gitignore
```

| Pasta ou arquivo | Para que serve |
|---|---|
| `README.md` | Explica o objetivo, como começar, estrutura e comandos principais |
| `AGENTS.md` ou `CLAUDE.md` | Dá instruções aos Agents que trabalham no projeto |
| `docs/` | Guarda PDFs, planilhas, requisitos, links e demais referências |
| `docs/fontes/` | Guarda os materiais originais usados no projeto |
| `data/raw/` | Dados originais, que não devem ser alterados |
| `data/processed/` | Dados limpos ou transformados |
| `notebooks/` | Experimentos e análises interativas |
| `src/` | Código principal reutilizável |
| `tests/` | Testes automáticos |
| `outputs/` | Relatórios, gráficos e arquivos gerados |
| `pyproject.toml` | Dependências e configurações do projeto Python |
| `.gitignore` | Lista arquivos que não devem ir para o Git |

### O que escrever no README

O `README.md` deve responder rapidamente:

1. O que é este projeto?
2. Qual problema ele resolve?
3. Onde está a documentação?
4. O que existe em cada pasta?
5. Como instalar e executar?
6. Como executar os testes?
7. Quais são as limitações conhecidas?

Prompt útil:

```text
Crie uma estrutura de projeto Python simples e fácil para iniciantes.
Inclua README.md, docs, data, notebooks, src, tests e outputs.
No README, explique o propósito de cada pasta e os comandos para instalar,
executar e testar. Não complique a arquitetura sem necessidade.
```

### Setup rápido para projetos descartáveis

Para testes, experimentos e projetos aleatórios que não precisam de Git, branches, CI ou estrutura formal, use o [`uv`](https://docs.astral.sh/uv/) — ele cuida sozinho do ambiente virtual, do Python e das dependências.

Verifique se o `uv` está instalado:

```bash
uv --version
```

Criar o projeto:

```bash
mkdir meu-projeto
cd meu-projeto
uv init
uv add pandas
```

Instalar outras bibliotecas:

```bash
uv add numpy matplotlib scikit-learn
```

Abrir no editor:

```bash
code .      # VS Code
cursor .    # Cursor
```

Executar:

```bash
uv run python main.py
```

Quando não precisar mais do experimento, basta apagar a pasta.

## 8. VS Code com Agents

O [Visual Studio Code](https://code.visualstudio.com/download) é um editor gratuito. Dentro dele, é possível instalar extensões de Agents pela própria tela de extensões.

| Extensão oficial | Instalação | Documentação |
|---|---|---|
| Claude Code | Buscar `Claude Code for VS Code` no painel de extensões | [Marketplace](https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code) |
| Codex | Buscar `Codex – OpenAI's coding agent` | [Marketplace](https://marketplace.visualstudio.com/items?itemName=openai.chatgpt) e [guia oficial](https://developers.openai.com/codex/ide) |
| Python | Buscar `Python`, publicada pela Microsoft | [Marketplace](https://marketplace.visualstudio.com/items?itemName=ms-python.python) |

### É preciso instalar Python antes?

| Situação | Resposta simples |
|---|---|
| Usar Colab | Não. O Python executa na nuvem. |
| Criar e executar `.py` no computador | Sim. Instale pelo [site oficial do Python](https://www.python.org/downloads/) e marque a opção de adicionar Python ao `PATH` no Windows. |
| Pedir ao Agent para instalar | Ele pode orientar e, com permissão, talvez executar parte da instalação. Para iniciantes, é melhor instalar pelo site oficial e pedir ao Agent para **verificar** a instalação. |

Prompt de verificação:

```text
Verifique se Python e Git estão instalados neste computador.
Não faça mudanças ainda. Mostre o que encontrou e explique em linguagem simples
qual instalação ou configuração falta.
```

## 9. Claude Code sem mistério

O [Claude Code](https://code.claude.com/docs/en/overview) é um Agent que lê o projeto, edita vários arquivos e executa comandos com permissão. A extensão do VS Code (instalada acima) oferece uma interface visual para o mesmo mecanismo.

### Tudo começa com arquivos Markdown

<span style="color: orange"><strong>Boa parte da personalização pode ser criada pedindo ao próprio Claude Code para escrever os arquivos necessários da forma que você quer.</strong></span>

| Local | Escopo | Exemplo de uso |
|---|---|---|
| `~/.claude/CLAUDE.md` | Preferências pessoais para todos os projetos | Idioma, estilo e hábitos de trabalho |
| `CLAUDE.md` ou `.claude/CLAUDE.md` | Instruções compartilhadas do projeto | Arquitetura, comandos e padrões |
| `.claude/rules/*.md` | Regras gerais ou aplicadas a certos caminhos | Regras para `src/` ou `tests/` |
| `.claude/agents/*.md` | Subagents personalizados do projeto | Revisor, pesquisador ou testador |
| `~/.claude/agents/*.md` | Subagents pessoais disponíveis em projetos | Worker reutilizável |
| `.claude/skills/<nome>/SKILL.md` | Skills reutilizáveis do projeto | Criar relatório ou revisar notebook |
| `.claude/settings.json` | Permissões, hooks e configurações compartilhadas | Permitir ou negar tools |
| `.claude/settings.local.json` | Configuração local, não compartilhada | Permissões específicas da máquina |

Links oficiais:

- [Memória, CLAUDE.md e rules](https://code.claude.com/docs/en/memory)
- [Criar subagents](https://code.claude.com/docs/en/sub-agents)
- [Criar skills](https://code.claude.com/docs/en/skills)
- [Visão geral das extensões](https://code.claude.com/docs/en/features-overview)
- [Configurações](https://code.claude.com/docs/en/settings)
- [Hooks](https://code.claude.com/docs/en/hooks)
- [Referência de tools](https://code.claude.com/docs/en/tools-reference)
- [Comandos do Claude Code](https://code.claude.com/docs/en/commands)

### Exemplo de CLAUDE.md simples

```markdown
# Instruções do projeto

- Responda em português brasileiro.
- Leia o README.md e os arquivos relevantes de docs/ antes de planejar.
- Mantenha a solução simples e adequada para iniciantes.
- Antes de editar, explique brevemente o plano.
- Não altere os dados originais em data/raw/.
- Sempre execute Ruff, mypy e pytest antes de concluir uma tarefa.
- Para código puro (funções, scripts de dados, protótipos), crie também um
  notebook de teste rápido em notebooks/ para validar o comportamento na prática,
  além dos testes automatizados.
- Sempre crie ou atualize um progress.md com as fases do plano e o status de
  cada uma (pendente, em andamento, concluída) antes de começar a implementar.
- Ao final de cada fase, marque-a como concluída em progress.md antes de
  seguir para a próxima.
- Atualize o README.md quando o modo de usar o projeto mudar.
```

Essas instruções orientam o modelo, mas não são uma barreira de segurança garantida. Para bloquear ações, use permissões e hooks.

<span style="color: orange"><strong>Use o próprio modelo para criar o CLAUDE.md (Claude Code) ou AGENTS.md (Cursor e outros).</strong></span>

### Agents internos principais

| Agent | Para que serve | Pode editar? |
|---|---|---:|
| Explore | Procura arquivos, entende o projeto e responde perguntas sobre o código | Normalmente não |
| Plan | Pesquisa e cria um plano antes da implementação | Não durante o planejamento |
| General-purpose | Resolve tarefas variadas usando as tools disponíveis | Depende das permissões |
| Agent personalizado | Executa uma função definida por você | Depende da configuração |

O Claude pode delegar automaticamente para um subagent quando a descrição combina com a tarefa. Para pedir um Agent específico, escreva claramente: `Use o subagent test-runner para executar e analisar os testes.`

**Sobre `@`:** use `@arquivo` ou `@pasta` para colocar arquivos e pastas no contexto. Não dependa de `@nome-do-agent` para invocar um subagent; essa não é a forma oficial e garantida. Peça pelo nome em linguagem natural.

### Tools principais

| Tool | O que faz |
|---|---|
| `Read` | Lê um arquivo |
| `Write` | Cria ou substitui um arquivo |
| `Edit` | Altera trechos de um arquivo |
| `Glob` | Encontra arquivos usando padrões de nomes |
| `Grep` | Procura texto dentro de arquivos |
| `Bash` ou `PowerShell` | Executa comandos no terminal |
| `WebSearch` | Pesquisa informações atuais na web |
| `WebFetch` | Lê uma página específica |
| `Agent` | Delega uma tarefa para um subagent |
| `NotebookEdit` | Modifica células de notebooks |

### Rules, skills e Agents: qual usar?

<span style="color: orange"><strong>Assim como o CLAUDE.md, os arquivos markdown (.md) de Rules, Skills e Subagents também podem ser escritos pelo próprio Agent: basta explicar o que você quer e pedir para ele criar o arquivo.</strong></span>

| Recurso | Use quando... | Exemplo |
|---|---|---|
| `CLAUDE.md` | A instrução deve aparecer em todas as sessões do projeto | `Use Python 3.14` |
| Rule | A instrução deve valer para uma área ou tipo de arquivo | Regras somente para `tests/**/*.py` |
| Skill | Existe um procedimento específico e reutilizável | Como gerar uma apresentação, cores a serem usadas etc. |
| Subagent | Um worker precisa de contexto próprio, papel e tools específicas | Revisor de segurança |
| Hook | Uma ação precisa acontecer de forma automática e determinística | Rodar o formatador após uma edição |

### Cinco comandos úteis

| Comando | Para que serve |
|---|---|
| `/help` | Mostra ajuda e comandos disponíveis |
| `/status` | Mostra modelo, conta e estado da sessão |
| `/memory` | Abre e gerencia instruções e memória |
| `/compact` | Resume uma conversa longa para liberar contexto |
| `/skills` | Lista as skills disponíveis |

Consulte a [lista oficial e atualizada de comandos](https://code.claude.com/docs/en/commands), pois ela muda conforme a versão.

## 10. Cursor para planejar e construir

O [Cursor](https://cursor.com/download) é um editor de código com Agent integrado. Ele é parecido com o VS Code e inclui modos para perguntar, planejar, implementar e depurar.

Links úteis:

- [Download do Cursor](https://cursor.com/download)
- [Quickstart](https://cursor.com/docs/get-started/quickstart)
- [Plan Mode](https://cursor.com/docs/agent/plan-mode)
- [Rules](https://cursor.com/docs/rules)
- [Documentação geral](https://cursor.com/docs)

### Use Plan Mode antes de uma feature maior

Selecione Plan Mode na janela do agente ou pressione `Shift + Tab` no campo de conversa até chegar ao Plan Mode. O Agent pesquisa o projeto, faz perguntas e cria um plano revisável antes de editar arquivos.

<span style="color: orange"><strong>Planejar antes de implementar reduz erros: o Agent entende melhor o pedido, você consegue corrigir uma direção errada antes que ela vire código, e ambos ficam alinhados sobre o que vai ser feito antes do trabalho começar. É muito mais barato ajustar um plano do que desfazer uma implementação inteira.</strong></span>

Prompt inicial:

```text
Entre em Plan Mode e planeje esta feature antes de editar qualquer arquivo.
Leia o README e a pasta docs. Faça perguntas se algum requisito estiver incerto.
Divida o plano em passos pequenos, inclua testes e espere minha aprovação.
```

### Dica: crie um `progress.md` para planos com várias fases

Quando o plano detalhado tiver várias fases (por exemplo: "Fase 1 — estrutura do projeto", "Fase 2 — backend", "Fase 3 — testes"), peça ao Agent para salvar esse plano em um arquivo `progress.md` na raiz do projeto, marcando o que já foi feito e o que falta.

Isso permite um **fluxo semi-autônomo** muito útil, especialmente em projetos maiores:

```text
Salve o plano aprovado em progress.md, com uma lista de fases e status
(pendente, em andamento, concluída). Atualize esse arquivo sempre que
terminar uma fase.
```

Depois, em vez de reexplicar o contexto a cada sessão, basta dizer:

```text
Continue para a próxima fase.
```

```text
Faça as fases 3 e 4 agora.
```

O Agent lê o `progress.md`, entende onde parou e continua sozinho, sem precisar que você reescreva o plano inteiro. Esse hábito também ajuda a retomar o trabalho depois de fechar o editor ou perder o contexto da conversa.

### Comandos principais do Cursor CLI

| Comando | Para que serve |
|---|---|
| `/plan` | Entrar em Plan Mode ou mostrar o plano atual |
| `/ask` | Fazer perguntas sem editar o projeto |
| `/debug` | Investigar um problema |
| `/model` | Selecionar o modelo |
| `/help` | Ver ajuda e comandos disponíveis |

Veja a [referência oficial de slash commands](https://cursor.com/docs/cli/reference/slash-commands).

As regras de projeto ficam em `.cursor/rules/` como arquivos `.mdc`. Um `AGENTS.md` simples também pode ser usado para instruções em Markdown.

## 11. Testes e qualidade para projetos de código

<span style="color: orange"><strong>Dica que melhora muito a qualidade dos resultados dos agentes: peça ao Agent para executar testes, ler os erros, corrigir o código e executar tudo novamente.</strong></span>

| Ferramenta | O que verifica | Link |
|---|---|---|
| Ruff | Estilo, erros comuns e organização do código Python | [Documentação](https://docs.astral.sh/ruff/) |
| mypy | Incompatibilidades de tipos antes da execução | [Documentação](https://mypy.readthedocs.io/) |
| pytest | Se as funções fazem o que deveriam | [Documentação](https://docs.pytest.org/) |

Guarde os testes em `tests/`. Eles ajudam o Agent a entender o comportamento esperado e reduzem a chance de uma correção quebrar algo que já funcionava.

Prompt útil:

```text
Crie testes simples em tests/ para os comportamentos principais.
Execute Ruff, mypy e pytest. Corrija os problemas encontrados e execute tudo novamente.
No final, explique em linguagem simples o que cada verificação confirmou.
Não esconda testes que falharam.
```

<span style="color: orange"><strong>Essas instruções também podem ficar salvas de forma permanente no `CLAUDE.md` ou `AGENTS.md` do projeto, para que o Agent execute testes automaticamente em todas as sessões, sem precisar repetir o prompt toda vez.</strong></span>

## 12. Projeto final sugerido

Escolha um tema que te interesse: Pokémon, futebol, filmes, música, livros, jogos ou astronomia.

| Entrega | Conteúdo mínimo |
|---|---|
| Pergunta | Uma pergunta clara que os dados conseguem responder |
| Dados | Uma tabela pequena com fonte registrada em `docs/fontes/` |
| Notebook | Leitura, filtro, resumo e um gráfico |
| Código | Uma função simples em `src/` |
| Testes | Pelo menos dois testes em `tests/` |
| Documentação | README com objetivo, pastas, execução e limitações |
| Apresentação | Cinco slides ou um resumo de uma página, criado com o Agent (ex.: peça um PPT ou uma página em Markdown) |
| Verificação | Uma lista do que foi conferido manualmente |

Fluxo recomendado:

1. Peça ao coordinator para ler o objetivo e criar um plano.
2. Use um worker de pesquisa para localizar os dados e registrar as fontes.
3. Use um worker de código para montar o notebook e a função.
4. Use um worker de qualidade para executar os testes e revisar a documentação.
5. Volte ao coordinator para juntar tudo e mostrar o resultado final.

Esse fluxo com coordinator e workers se aplica diretamente ao Grok Bot. No Claude Code ou no Cursor, basta pedir cada etapa normalmente na conversa principal (o próprio Agent já organiza os passos); a menção ao coordinator só faz sentido se você já tiver criado subagents específicos para o projeto.

## 13. Segurança e bons hábitos

| Faça | Evite |
|---|---|
| Confira fatos importantes em fontes confiáveis | Confiar em uma resposta só porque está bem escrita |
| Leia o plano antes de aprovar mudanças | Liberar acesso total sem entender a necessidade |
| Use arquivos de exemplo sem dados pessoais | Enviar senhas, documentos, dados escolares ou informações privadas |
| Faça backups e versões com Git | Deixar o Agent apagar ou substituir grandes pastas sem revisão |
| Comece com permissões pequenas | Conectar todas as contas logo no primeiro teste |
| Revise mensagens e arquivos antes de enviar | Permitir envios externos automáticos durante o aprendizado |

## 14. Bônus: Git e GitHub

O Git cria versões do projeto. O GitHub guarda repositórios online e facilita colaboração, revisão e compartilhamento.

<span style="color: orange"><strong>Esta seção é voltada para quem quer aprender a programar de forma mais estruturada, duradoura e com boas práticas, e não apenas fazer projetos pessoais ou descartáveis.</strong></span> Se o objetivo é só testar ideias rapidamente, o [setup com `uv`](#setup-rápido-para-projetos-descartáveis) do item 7 é suficiente.

Links para começar:

- [Download do Git](https://git-scm.com/downloads)
- [Livro Pro Git em português](https://git-scm.com/book/pt-br/v2)
- [Documentação do GitHub em português](https://docs.github.com/pt/get-started)
- [Criar uma conta no GitHub](https://github.com/signup)

### Comandos fundamentais

| Comando | Significado simples |
|---|---|
| `git status` | Mostra o que mudou |
| `git add .` | Seleciona mudanças para a próxima versão |
| `git commit -m "mensagem"` | Cria uma versão local com uma descrição |
| `git push` | Envia as versões para o repositório remoto |
| `git pull` | Baixa e combina mudanças do remoto |
| `git branch` | Lista ou cria linhas de trabalho |
| `git merge` | Combina o trabalho de uma branch em outra |

### Três ambientes comuns

| Ambiente | Para que serve | Regra simples |
|---|---|---|
| Desenvolvimento local | Criar e testar mudanças no computador | Pode mudar com frequência |
| Homologação ou staging | Conferir a versão quase final | Deve ser parecida com produção |
| Produção | Versão usada pelo público | Só recebe mudanças revisadas e testadas |

Branches do Git não são exatamente a mesma coisa que ambientes, mas ajudam a controlar qual versão será testada ou publicada em cada um; um ambiente, por sua vez, é a infraestrutura real (servidor, hardware ou serviço em nuvem) onde essa versão roda de fato.

## Checklist de conclusão

- [ ] Criei e melhorei prompts em pelo menos duas plataformas.
- [ ] Consigo explicar a diferença entre chat, Agent, tool, skill e rule.
- [ ] Sei que as plataformas têm nomes diferentes, mas capacidades parecidas.
- [ ] Criei um coordinator e workers especializados.
- [ ] Experimentei colaboração entre Bots ou subagents.
- [ ] Abri, executei e modifiquei um notebook no Colab.
- [ ] Montei uma estrutura de pastas clara e escrevi um README.
- [ ] Usei um Agent no VS Code ou no Cursor.
- [ ] Pedi um plano antes de uma mudança maior.
- [ ] Executei testes e conferi o resultado.
- [ ] Entendi o básico de Git e criei pelo menos um commit.
- [ ] Consigo mostrar um projeto pequeno e explicar o que a IA fez e o que eu conferi.

## Próximos passos opcionais

Depois desta trilha, escolha apenas uma direção:

| Interesse | Próximo passo |
|---|---|
| Estudo | Criar uma skill de tutor que use materiais da disciplina |
| Dados | Aprender pandas e visualização com um dataset pequeno |
| Programação | Criar uma aplicação simples com interface |
| Automação | Estudar rotinas, MCP e integrações com cuidado |
| Trabalho em equipe | Aprofundar Git, GitHub, branches e pull requests |
| Agents | Criar subagents com tools e permissões específicas |

O objetivo não é dominar todas as plataformas, mas conseguir começar um projeto, orientar um Agent, entender o que ele fez, testar o resultado e continuar aprendendo sozinho. Com isso, você facilita tarefas do dia a dia e amplia o campo em que consegue atuar.
