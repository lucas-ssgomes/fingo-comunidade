# Fingo — o agente do FING para as coordenações e a Comunidade

> Este arquivo é o contexto que o Claude lê toda vez que você abre uma conversa nesta pasta.
> É o que faz ele conhecer o FING sem você ter que explicar tudo de novo a cada sessão.
>
> **Versão pública**, mantida pela Coordenação Geral e distribuída por release.
> **Não edite este arquivo** esperando que a mudança volte para todo mundo — ela some no
> próximo release. Para propor correção, fale com a Coordenação Geral.

**Idioma de trabalho:** português (pt-BR), em tudo — textos, comentários e anotações.
**Versão do pacote:** `v2026.4`

---

## Como usar

Peça em português normal, sem comando especial. O Claude escolhe a habilidade certa sozinho:

| Quando você quer | Peça assim |
|---|---|
| Escrever um post, legenda, e-mail, convite ou release | "escreve um post de Instagram sobre..." |
| Saber se um texto pronto está no tom do FING | "esse texto está no tom?" + cole o texto |
| Planejar ou priorizar a frente de Comunicação | "o que a Comunicação precisa entregar essa semana?" |
| Planejar a grade, palestrantes, pitches ou oficinas | "como distribuo essas palestras entre os palcos?" |
| Planejar estrutura, escalas, montagem ou riscos | "monta a escala do credenciamento" |
| Conduzir a coordenação, os ritos e as prioridades | "o que só a Coordenação Geral pode destravar essa semana?" |
| Preparar abordagem a patrocinador ou avaliar contrapartida | "como priorizo a fila de prospecção?" |
| Saber se uma atividade cabe no orçamento | "quanto custa botar mais uma palestra no Cinema?" |
| Descobrir o que está travando o quê | "o que está travado esperando outra coordenação?" |
| Um parecer independente sobre uma peça pronta | "manda o guardião da narrativa olhar isso" |

> ⚠️ **A regra que mais importa:** o Claude **não inventa frase de efeito** para o FING.
> A narrativa já existe, foi escrita pela Duda e refinada pela Coordenação Geral. Ele usa o
> banco de frases oficial. Se faltar frase para um caso novo, ele diz que falta em vez de
> inventar — e aí a decisão é de quem coordena, não dele.

---

# PARTE 1 — O que vale para qualquer edição

## O evento

**FING — Festival de Inovação e Negócios de Garanhuns.** Entrada gratuita, um dia,
no Centro Cultural do Sesc Garanhuns, realizado pela **Comunidade Sete Colinas** com
co-realização do **Sesc** e do **Sebrae/PE**.

**Inovação não é um pilar que vai para um palco.** Está dentro da sigla, então é tema
presente em **todo o evento, em todos os palcos e espaços**. Os outros pilares variam de
edição para edição. Na prática: uma mulher que fala de inovação **já contempla**
Empreendedorismo Feminino, mesmo que a planilha da programação não a classifique assim.

## As coordenações e as interfaces entre elas

A estrutura das frentes, o que cada uma responde e — o mais importante — **onde uma depende
da outra** está em [`docs-base/governanca-coordenacoes-fing26.md`](docs-base/governanca-coordenacoes-fing26.md).
Leia antes de assumir que algo é da sua frente ou da de outro. O mesmo arquivo traz as
**regras que valem para todas as frentes** — jurídico antes de assinar, nada colado na parede
do Sesc, político fora do palco, tráfego pago só a partir de outubro, entre outras.

Onde cada assunto se fala está em
[`docs-base/descricoes-grupos-whatsapp.md`](docs-base/descricoes-grupos-whatsapp.md).

## Narrativa e tom — leia antes de escrever qualquer peça

| Arquivo | O quê |
|---|---|
| [`docs-base/storytelling-fing26.md`](docs-base/storytelling-fing26.md) | A história: narrativa central, tensão, promessa, manifesto, pilares, personas e o **banco de frases** |
| [`docs-base/tom-e-voz-fing26.md`](docs-base/tom-e-voz-fing26.md) | Como falamos: personalidade, o que evitar, tom por público, checklist |

**O balizador é o `tom-e-voz`.** É ele que decide se um texto está certo ou errado.
O `storytelling` guarda a narrativa e as frases prontas que você pode usar.

A **assinatura da realização, as hashtags da série e as grafias fixas** das legendas estão na
tabela de fatos da habilidade de escrita (`.claude/skills/escrever-peca/`) — o Claude já
aplica sozinho.

## O prédio: Centro Cultural do Sesc Garanhuns

[`docs-base/infraestrutura-sesc-garanhuns.md`](docs-base/infraestrutura-sesc-garanhuns.md)
traz a capacidade oficial de cada espaço, os riders técnicos, a acessibilidade e as regras
de uso, extraídos do portfólio oficial do Sesc.

⚠️ **Capacidade de portfólio é o teto do espaço, não a configuração do FING.** O Auditório
comporta 200 pessoas vazio; em 2026 ele foi dividido ao meio e a metade de palestras ficou
com 130 lugares. Sempre confira a configuração do ano antes de usar um número.

⚠️ **O espaço é cedido, não alugado.** Onde se pode pregar, colar ou pendurar **não é decisão
do FING**. Pergunte ao Sesc antes de planejar qualquer fixação.

## O dinheiro: o que custa e quem decide

[`docs-base/orcamento-para-coordenador.md`](docs-base/orcamento-para-coordenador.md) traz o
custo de cada espaço e de cada bloco do evento, as regras de gasto, **quando uma atividade
nova pode ser vetada** e o tamanho do time.

A regra que resolve quase tudo: **todo item tem uma fonte que o paga, e "a captar" não é
dinheiro em caixa**. Antes de prometer qualquer coisa a alguém, confirme com a Coordenação
Geral se a fonte daquele item já está garantida.

⚠️ **O quadro de captação não está aqui** — quanto falta fechar, a tabela de cotas, os
valores por patrocinador e as negociações em andamento ficam no canal fechado de Negócios.
Cifra de negociação em aberto muda de lado quando circula.

## Ampliar o contexto com o Drive da Comunidade

Se você já tem acesso ao Drive da Comunidade, dá para conectá-lo ao seu Claude e trabalhar
com os arquivos vivos junto deste pacote —
[`docs-base/fontes-da-comunidade.md`](docs-base/fontes-da-comunidade.md) explica como, para
quem funciona, e as **três regras de cuidado** com o que existe lá (a planilha de curadoria
tem contato de mais de 100 pessoas, muitas ainda não abordadas).

> 🔄 **Mudou em 20/09/2026: a planilha financeira do Drive é a matriz**, não uma cópia
> publicada. É o arquivo vivo do planejamento de custos da edição. Quem tem acesso de edição
> e encontrar um erro **pode corrigir ali mesmo** — é justamente para permitir revisão a mais
> de uma mão que ela fica lá. Avise a Coordenação Geral do que mudou, para o registro
> versionado acompanhar.

## A régua de prazo

Sprints **semanais** — [`todo/sprints.md`](todo/sprints.md). A reunião da coordenação é o
único momento em que prazo se pactua ou se repactua; item levantado no meio da semana entra
na sprint seguinte.

O **dia da reunião é escolha de cada edição**, não regra fixa: em 2026 ficou na terça-feira,
por ter sido o melhor dia para os coordenadores desta edição.

Crie seus próprios arquivos de pendência dentro de [`todo/`](todo/) — o agente
`radar-de-prazos` lê essa pasta para dizer o que está travando o quê.

---

# PARTE 2 — A edição de 2026

> Esta parte envelhece. Quando 2026 acabar, ela vira lições aprendidas e a Parte 1 continua
> de pé para a edição seguinte.

| | |
|---|---|
| Data | Sábado, **28 de novembro de 2026** |
| Local | Centro Cultural do Sesc Garanhuns |
| Montagem / desmontagem | 27/11 e 29/11 |
| Entrada | Gratuita |
| Meta de inscritos | **3.000** |
| Público esperado no local | ~2.000 |
| Inscrições | **Sympla** — abrem **sexta, 25/09/2026, à noite** |
| Chamada aberta de conteúdo | Sai **quinta, 24/09, à noite** — propostas até **08/10**, resultado em **17/10** |

**Slogan oficial:** **"Agreste Conectado, Berço de Inovação"** (Mídia Kit de 11/08).
A variante "Próspero de Inovação" está **descontinuada** — não use.

**Os cinco pilares de 2026:** Inovação · Pessoas e Comunidades · Economia Criativa ·
Sustentabilidade · Empreendedorismo Feminino.

## Os palcos

| Palco | Capacidade | Formato |
|---|---|---|
| **Teatro** Reinaldo de Oliveira | 496 (mezanino incluso) | **Palco principal:** abertura, encerramento, magnas, keynotes e entrevistas. **É aqui que ficam as flâmulas.** Mestres de cerimônia: Dani e Emanuel |
| **Auditório** (metade esquerda) | 130 — 100 cadeiras + 30 almofadas | Palestras, painéis, mesas redondas e rodas de conversa, com escuta silenciosa |
| **Cinema** | 152 | Projeção DCP 2K e Dolby 5.1, mas **limitada** — ver abaixo |
| **Mezanino** (aquário do 2º nível) | 70 | **O palco mais intimista:** puffs, almofadas e a plateia perto de quem apresenta. Escuta silenciosa |

⚠️ **O "Mezanino" não é o mezanino do Teatro** — é outro espaço, o aquário do 2º nível.
E **só comporta dois formatos**: palestra e entrevista entre duas pessoas. O palco é
pequeno; mesa redonda e painel não cabem ali.

⚠️ **Não programe slides no Cinema.** A sala projeta por câmera cinematográfica e não recebe
bem conteúdo comum. O uso recomendado é só **vídeo de patrocinador no intervalo**, o
**motion** dos patrocinadores e a **tela de descanso** do evento. Atividade que dependa de
PPT precisa de **projetor separado** — foi o que se fez em 2025, e o projetor teve que ficar
no meio da plateia para alcançar a tela. Se a palestra tem slides, prefira outro palco.

⚠️ **Os nomes dos 4 palcos ainda não foram definidos**, e isso trava as artes e a
sinalização. Ficou combinado que **não** serão os pilares temáticos. A decisão sai até **23/09 à
noite** — no limite, **24/09 de manhã** —, porque a decoração começa em 24/09. A **Arena de
Startups** já tem conceito: **ringue de boxe**.

## Os outros espaços

| Espaço | O quê |
|---|---|
| **Credenciamento** | No Aquário, na entrada dos vidros |
| **Arena de Startups** | Metade **direita** do Auditório dividido — 18 startups, batalha de pitch e matchmaking do Sebrae |
| **Área de Ativações** (Hall) | Stands das marcas. O Hall é **só circulação, fila e visita** — não há lugar para sentar |
| **Lounge de Negócios** (2º andar) | Restrito a palestrante, expositor, patrocinador e organização, por QR code no crachá |
| **Corredor da Comunidade** (1º andar) | Linha do tempo dos 8 anos da Sete Colinas, mentorias e ativações |
| **Salas de oficina** | 6 salas, ~20 pessoas cada, uso simultâneo. Inscrição separada, com certificado |

**Show de encerramento:** 1h30, produzido pelo Sesc, com artista do Agreste a definir.

**Acessibilidade:** 8 intérpretes de Libras, 2 por palco.

## O que está travado agora

- 🔴 **Os nomes dos 4 palcos** — travam 7 peças gráficas com prazo de gráfica em outubro
- 🔴 **Conteúdo é o gargalo declarado:** 15 palestrantes confirmados contra uma meta de ~50.
  A chamada aberta de palestrantes e oficineiros sai **quinta, 24/09, à noite**: propostas de
  24/09 a 08/10, análise até 15/10 e resultado em 17/10. A participação é voluntária, a
  prioridade é para quem é de Garanhuns, Caruaru e do Agreste, e **toda proposta passa pela
  curadoria** — não prometa vaga a ninguém. ⚠️ Aqui não há pontuação regional: ela é só do
  edital de startups

## Duas regras novas (22/09)

- **Post de patrocinador só depois do contrato assinado.** Nenhuma marca aparece nas redes
  antes disso, por mais adiantada que a conversa esteja. A entrega por cota, depois da
  assinatura: **Master** vídeo de retrospectiva exclusivo + collab · **Ouro** 3 fotos em
  carrossel · **Prata** 1 post com logo · **Bronze** carrossel coletivo.
- **A prestação de contas fecha até 31/12** — o último dia útil do ano. Cobre fornecedores,
  notas fiscais, vídeos de agradecimento, After Movie e a **comprovação de cada contrapartida**
  entregue a patrocinador. Comprovação se guarda **no dia do evento** — foto da marca no palco,
  print do post, lista de presença —, porque reconstruir em dezembro custa bem mais. Se a sua
  frente entrega contrapartida, planeje o registro junto com a entrega.

---

## O que NÃO está neste pacote, e por quê

O **quadro de captação** — quanto falta fechar, a tabela de cotas, valores por patrocinador,
negociações em andamento e o histórico das edições anteriores. Mais os **contratos**, os
**dados de fornecedor** e as **transcrições de reunião**.

Não é desconfiança. São duas razões concretas: cifra de negociação em aberto **muda de lado
quando circula** — quem senta do outro lado da mesa passa a saber o quanto precisamos —, e
contrato e transcrição envolvem dados de terceiros que não cabe distribuir.

O que **está** aqui é o que muda decisão de coordenação: o custo de cada parte do evento, as
regras de gasto e o tamanho do time.

Se a sua frente precisa de um número que ficou do outro lado, **peça** — a resposta vem, só
não vem por download.
