# Fingo — Comunidade

**O agente que ajuda as coordenações e os voluntários do FING a trabalhar.**

O FING — Festival de Inovação e Negócios de Garanhuns — é organizado por voluntários da
**Comunidade Sete Colinas**, em parceria com o Sesc e o Sebrae. O Fingo é um assistente que
já conhece o evento: a narrativa, o tom de voz, o prédio do Sesc, a estrutura das
coordenações e o que está acontecendo nesta edição.

Na prática, ele serve para você **não começar do zero** toda vez que precisar escrever um
post, planejar a sua frente ou descobrir o que está travando o seu trabalho.

> **Versão do pacote:** `v2026.2.1` · **Edição:** FING 2026 (28 de novembro de 2026)

---

## Índice

- [O que dá para pedir a ele](#o-que-dá-para-pedir-a-ele)
- [Como usar — escolha o seu caminho](#como-usar--escolha-o-seu-caminho)
  - [Caminho 1 — Claude Code (o mais completo)](#caminho-1--claude-code-o-mais-completo)
  - [Caminho 2 — Project no Claude Desktop ou no navegador](#caminho-2--project-no-claude-desktop-ou-no-navegador)
  - [Caminho 3 — anexar arquivos numa conversa](#caminho-3--anexar-arquivos-numa-conversa-quebra-galho)
- [Qual caminho é o seu](#qual-caminho-é-o-seu)
- [Ampliar o contexto com o Drive](#ampliar-o-contexto-com-o-drive-da-comunidade)
- [O primeiro teste](#o-primeiro-teste)
- [O que ele não sabe, de propósito](#o-que-ele-não-sabe-de-propósito)
- [Atualizações e versões](#atualizações-e-versões)
- [Achou um problema? Abra uma Issue](#achou-um-problema-abra-uma-issue)

---

## O que dá para pedir a ele

Em português normal, sem comando especial:

| Quando você quer | Peça assim |
|---|---|
| Escrever post, legenda, e-mail, convite ou release | "escreve um post de Instagram sobre a chamada de palestrantes" |
| Saber se um texto pronto está no tom do FING | "esse texto está no tom?" + cole o texto |
| Planejar ou priorizar Comunicação | "o que a Comunicação precisa entregar essa semana?" |
| Planejar grade, palestrantes, pitches ou oficinas | "como distribuo essas palestras entre os palcos?" |
| Planejar estrutura, escalas, montagem ou riscos | "monta a escala do credenciamento" |
| Conduzir a coordenação e as prioridades | "o que só a Coordenação Geral pode destravar?" |
| Preparar abordagem a patrocinador, avaliar contrapartida | "como priorizo a fila de prospecção?" |
| Saber se uma atividade cabe no orçamento | "quanto custa botar mais uma palestra no Cinema?" |
| Descobrir o que está travando o quê | "o que está travado esperando outra coordenação?" |
| Um parecer independente sobre uma peça pronta | "manda o guardião da narrativa olhar isso" |

> ⚠️ **A regra que mais importa:** o Fingo **não inventa frase de efeito** para o FING. A
> narrativa já existe — foi escrita pela Duda e refinada pela Coordenação Geral. Ele usa o
> banco de frases oficial, e quando falta frase para um caso novo, ele **diz que falta** em
> vez de inventar. Se você vir ele produzindo "chamada de pertencimento" inédita, algo está
> errado: avise pela Issue.

---

## Como usar — escolha o seu caminho

Os três caminhos funcionam. Eles não funcionam **igual**, e vale saber a diferença antes de
escolher.

### Caminho 1 — Claude Code (o mais completo)

É o Claude que roda no seu computador e enxerga a pasta inteira. **É o único caminho em que
tudo funciona automaticamente**: ele lê o contexto do FING sozinho, escolhe a habilidade
certa para o que você pediu e chama os agentes quando precisa.

Está incluído no **plano Pro**. Funciona no terminal ou dentro do VS Code.

```bash
# 1. Instale o Claude Code (uma vez só)
npm install -g @anthropic-ai/claude-code

# 2. Baixe o pacote
git clone https://github.com/lucas-ssgomes/fingo-comunidade.git

# 3. Entre na pasta e abra
cd fingo-comunidade
claude
```

Pronto. Pergunte em português — não há comando para decorar.

**Se você não tem o `git` ou não quer usar terminal para baixar:** pegue o `.zip` em
[Releases](../../releases), descompacte, e abra a pasta com o `claude` de dentro dela.

**Vantagem:** funciona como foi desenhado, sem você configurar nada.
**Requisito:** instalar um programa e usar o terminal. Se isso te trava, vá para o Caminho 2.

---

### Caminho 2 — Project no Claude Desktop ou no navegador

Funciona bem, mas **exige um passo de configuração que não dá para pular**. Vale a pena ler
os cinco passos até o fim antes de começar.

1. Baixe o `.zip` da versão mais recente em **[Releases](../../releases)** e descompacte
2. No [claude.ai](https://claude.ai) ou no Claude Desktop, crie um **Project** chamado `FING`
3. **Abra o arquivo `CLAUDE.md`, copie o conteúdo inteiro e cole nas *Instruções do
   projeto*** (o campo de instruções personalizadas do Project)
4. Arraste **todos os outros arquivos** para o conhecimento do Project — as pastas
   `docs-base/`, `.claude/skills/`, `.claude/agents/` e `todo/`
5. Comece a conversar dentro do Project

> 🔴 **O passo 3 é o que faz funcionar.** Se você só arrastar os arquivos sem colar o
> `CLAUDE.md` nas instruções, o Claude vai tratar tudo como documento de consulta e **pode
> simplesmente não abrir** o guia de tom de voz na hora de escrever. O resultado sai com
> cara de texto genérico de IA — exatamente o que a gente quer evitar.

**As limitações honestas deste caminho:**

- **As habilidades não se ativam sozinhas.** No Claude Code, pedir "escreve um post" aciona
  a habilidade de escrita automaticamente. Aqui, não. O Claude busca nos arquivos por
  semelhança — e pode trazer o arquivo errado, ou nenhum.
- **A solução é simples: chame pelo nome.** Em vez de "escreve um post", peça *"usando o
  guia de tom e voz e o banco de frases, escreve um post"*. Funciona quase tão bem.
- **Os agentes viram documento.** `guardiao-da-narrativa` e `radar-de-prazos` não rodam como
  agentes separados aqui. Você pode pedir *"siga o guardião da narrativa e revise isto"* e
  ele segue as instruções — só não é um segundo par de olhos independente.
- **Atualizar dá trabalho.** A cada versão nova você refaz os passos 3 e 4. Não é
  automático como o `git pull`.

---

### Caminho 3 — anexar arquivos numa conversa (quebra-galho)

Dá para anexar dois ou três arquivos direto numa conversa avulsa, sem Project.

**Serve para:** uma pergunta pontual, uma vez só.
**Não serve para trabalhar.** Tudo se perde quando a conversa acaba, e você vai reanexar
os mesmos arquivos toda vez. Se você vai usar o Fingo mais de uma vez por semana, gaste os
dez minutos do Caminho 2.

---

## Qual caminho é o seu

| Se você… | Vá para |
|---|---|
| Está confortável com terminal, ou usa VS Code | **Caminho 1** |
| Usa o Claude pelo navegador ou pelo app, e vai usar o Fingo com frequência | **Caminho 2** |
| Só quer testar, ou precisa de uma coisa pontual | **Caminho 3** |

Na dúvida, comece pelo **Caminho 2**. Ele cobre bem a maior parte do trabalho e não exige
instalar nada.

---

## Ampliar o contexto com o Drive da Comunidade

Este pacote traz o repertório que cabe circular. O material de trabalho vivo — planilha de
curadoria, documentos de coordenação, materiais das edições anteriores — mora no **Google
Drive da Comunidade**, na pasta `FINGs`.

**Se você já tem acesso a essa pasta**, vale ligar o **conector do Google Drive** no Claude
Desktop ou no claude.ai: você passa a trabalhar com os arquivos vivos junto deste pacote, e
a janela de contexto do Fingo fica bem maior.

O passo a passo está em
[`docs-base/fontes-da-comunidade.md`](docs-base/fontes-da-comunidade.md) — inclusive o erro
mais comum, que é autorizar a conta Google errada.

> 🔴 **Leia as três regras de cuidado nesse arquivo antes de usar.** O Drive **não passou
> pelo filtro que este pacote passou**: a planilha de curadoria tem e-mail e telefone de mais
> de 100 pessoas, muitas ainda nem abordadas. Não peça para o Claude listar contatos, e nada
> de lá vai para peça pública sem passar pela coordenação responsável.

**Não tem acesso à pasta?** O conector não cria permissão — peça acesso à Coordenação Geral
primeiro.

---

## O primeiro teste

Seja qual for o caminho, teste com isto:

> escreve um post de Instagram convidando para a chamada de palestrantes

**Está funcionando** se o texto usar o vocabulário do FING e as frases oficiais.
**Não está** se vier com frase motivacional genérica, "venha fazer parte dessa energia
transformadora" e afins. Nesse caso, no Caminho 2, peça de novo citando o guia de tom e voz
pelo nome. Se continuar, [abra uma Issue](../../issues).

---

## O que ele não sabe, de propósito

Desde a `v2026.2`, ele **sabe** o que custa cada parte do evento, as regras de gasto, quando
uma atividade pode ser vetada e o tamanho do time.

O que continua fora é o **quadro de captação**: quanto falta fechar, a tabela de cotas,
valores por patrocinador, negociações em andamento e o histórico das edições anteriores —
mais contratos, dados de fornecedor e transcrições de reunião.

A razão é concreta: **cifra de negociação em aberto muda de lado quando circula.** Quem senta
do outro lado da mesa passa a saber o quanto precisamos, e isso custa dinheiro ao evento.

Se ele disser que não tem essa informação, está certo — não insista nem peça para ele
estimar. **Peça o número à Coordenação Geral**, que a resposta vem.

---

## Atualizações e versões

O FING anda rápido: palcos ganham nome, prazos mudam, a narrativa é refinada, novas
habilidades entram. **Cada mudança relevante vira uma versão nova**, publicada em
[Releases](../../releases) com a lista do que mudou.

**Como atualizar:**

| Como você instalou | Como atualiza |
|---|---|
| `git clone` (Caminho 1) | `git pull` dentro da pasta |
| `.zip` (Caminhos 1, 2 e 3) | Baixe o release novo, e substitua os arquivos — no Caminho 2, refaça os passos 3 e 4 |

**Como saber se a sua versão está velha:** compare o número no topo deste arquivo com o
último release. Vale conferir antes de produzir qualquer peça que vá para fora.

### O que mudou na v2026.2.1

Atualização **incremental** — o terceiro número indica correção e ajuste, não pacote novo:
nada do que você já usa mudou de lugar.

O que entra é uma mudança de regra sobre o **financeiro no Drive**: aquela planilha passou a
ser a **matriz** do planejamento de custos, não mais um espelho publicado. Na prática, quem
tem acesso de edição e achar um erro **pode corrigir ali mesmo** — antes a orientação era o
contrário, confirmar com a Coordenação Geral em vez de mexer.

A razão é simples: mais de uma pessoa revisa esses números, e o lugar onde se corrige tem que
ser o lugar onde todo mundo olha. Avise a Coordenação Geral do que mudar, para o registro
acompanhar.

🔴 **Correção de número, se você usou a `v2026.2` para calibrar alguma proposta:** a tabela
de custos trazia a **Arena de Startups por R$37.782** na coluna *Custo de estrutura*. Estava
somando ali os **R$20.000 da premiação da Batalha de Pitches**, que é prêmio em dinheiro e
depende de patrocínio específico — não é estrutura. Isso fazia a Arena parecer o espaço mais
caro do evento, e ela não é: **a estrutura dela custa R$17.782**, quase o mesmo que o Teatro.
Se você dimensionou algo para a Arena pela versão anterior, **refaça a conta com R$17.782.**

### O que mudou na v2026.2

Entraram a habilidade de **Negócios**, a síntese de **orçamento para coordenador** (custos
por espaço e por bloco, regras de gasto e tamanho do time) e o guia para **conectar o Drive
da Comunidade**.

### O que vem a seguir

Mais contexto sintetizado a partir do Drive, conforme as frentes pedirem. **Diga o que faltou
para a sua** — é por isso que existe a seção abaixo.

Depois de 2026, o pacote continua: a parte permanente (narrativa, tom, o prédio, a
estrutura das coordenações, o método) atravessa as edições, e o que é específico de 2026
vira **lições aprendidas** para a edição seguinte.

---

## Achou um problema? Abra uma Issue

Encontrou informação errada, desatualizada, ou faltando? Achou que o Fingo respondeu mal?
Tem ideia de habilidade nova que ajudaria a sua frente?

**[Abra uma Issue](../../issues/new)** — é o canal para relatar e contribuir. Se puder,
inclua:

- **O que você pediu** (pode colar o texto)
- **O que ele respondeu** (ou o trecho errado)
- **O que era o certo**, se você souber
- **Qual caminho** você está usando (1, 2 ou 3) e qual versão do pacote

Isso vale ouro: é assim que a próxima versão sai melhor para todo mundo.

> ⚠️ **Não adianta corrigir o arquivo aqui e salvar.** Este repositório é **gerado** a partir
> da base de trabalho da Coordenação Geral — qualquer edição feita direto aqui some no
> próximo release. Por isso o caminho é a Issue: ela chega em quem consegue corrigir na
> origem.

---

*Mantido pela Coordenação Geral do FING · Comunidade Sete Colinas*
