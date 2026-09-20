# Ampliar o contexto com o Drive da Comunidade

> Este pacote traz o que **cabe circular**. O material de trabalho vivo do FING — planilhas
> de curadoria, documentos de coordenação, materiais das edições anteriores — mora no Google
> Drive da Comunidade Sete Colinas.
>
> Se você **já tem acesso** a esse Drive, dá para ligá-lo ao seu Claude e trabalhar com as
> duas coisas ao mesmo tempo: o repertório daqui e os arquivos vivos de lá.

## Para quem isso funciona

**Só para quem já tem acesso à pasta.** O conector não dá permissão nova — ele usa a que a
sua conta Google já tem. Se você não enxerga a pasta no seu Drive hoje, **peça acesso à
Coordenação Geral antes**; conectar não vai resolver.

A pasta é a **`FINGs`**, que contém uma subpasta por edição (`FING 2025`, `FING 2026`).

## Como ligar

Nas versões do Claude com conectores — **Claude Desktop** e **claude.ai no navegador**:

1. Abra as **configurações** e vá em **Conectores** (ou *Connectors*)
2. Ligue o **Google Drive**
3. Autorize **com a conta Google que tem acesso à pasta** — este passo é o que mais dá errado
4. Peça algo que dependa do Drive, citando o arquivo pelo nome

> 🔑 **Autorize a conta certa.** Se você tem mais de uma conta Google (pessoal, trabalho,
> faculdade), o acesso à pasta está em **uma** delas. Autorizar a outra faz o conector ligar
> normalmente e não achar nada — e o sintoma parece falta de arquivo, não conta errada.

**No Claude Code**, o caminho é outro: o conector do Drive não entra pela interface. Continue
usando o pacote local e, se precisar de um arquivo do Drive, baixe-o para a pasta.

## Como pedir para dar certo

Citar o arquivo pelo nome funciona muito melhor que pedir em termos gerais:

- ✅ *"Na planilha **Curadoria FING_2026_organizada**, quantos palestrantes estão confirmados por pilar?"*
- ❌ *"Quantos palestrantes temos?"* — ele não sabe onde procurar

## 🔴 Antes de usar: a parte que não é opcional

Os arquivos do Drive **não passaram pelo filtro que este pacote passou**. Ali existe
informação que não circula: dados pessoais de terceiros, valores em negociação e documentos
internos.

O caso mais sensível é a **planilha de curadoria**: ela tem **e-mail, telefone e LinkedIn de
mais de 100 pessoas** que foram mapeadas como possíveis palestrantes — muitas sequer
abordadas ainda.

**Três regras, quando estiver trabalhando com o Drive conectado:**

1. **Não peça para o Claude listar ou copiar contatos.** Trabalhe com contagens, status e
   nomes — não com e-mail e telefone de ninguém.
2. **Nada do Drive vai para peça pública** sem passar pela coordenação responsável. Nome de
   palestrante não confirmado em post é o erro clássico, e ele queima o convite.
3. **Pessoa mapeada não é pessoa convidada.** Estar na planilha significa que alguém pensou
   nela. Tratar como convite já feito gera constrangimento com quem nunca foi procurado.

## O que existe na pasta, por assunto

| Assunto | O que tem | Para quem serve |
|---|---|---|
| **Curadoria** | A planilha viva de palestrantes, com painel por pilar e grades horárias por palco; a Chamada Aberta de Propostas; o histórico da edição anterior | Conteúdo |
| **Patrocínio** | Materiais de captação e a prestação de contas da edição anterior | Negócios e Geral |
| **Financeiro** | O espelho publicado do planejamento financeiro | Geral |
| **Governança** | O Panorama Geral consolidado e o descritivo de coordenações | Todas |
| **Edições anteriores** | A pasta da edição passada, inteira | Todas, como referência |

> ⚠️ **O espelho financeiro do Drive é publicação, não origem.** Ele reflete o que a
> Coordenação Geral importou por último. Se um número parecer estranho, confirme com ela em
> vez de tratar a planilha do Drive como palavra final.

## Estado da curadoria (19/09/2026)

Útil para Conteúdo dimensionar o trabalho que falta, sem abrir a planilha:

| Pilar | Pessoas mapeadas |
|---|---|
| Inovação | 59 |
| Economia Criativa | 17 |
| Pessoas e Comunidades | 14 |
| Sustentabilidade | 11 |
| Empreendedorismo Feminino | 7 |
| Não classificado | 7 |
| **Total** | **115** |

Cada pessoa tem um status: `Confirmado`, `Convite feito`, `Em contato no LinkedIn`,
`Falta confirmar disponibilidade na data`, `Fazer convite no Instagram`, ou vazio — que
significa **mapeada, mas ainda não abordada**.

> 📌 **O número de confirmados sai de contar os status na planilha**, não de memória nem
> deste documento. Mapeado e confirmado são coisas muito diferentes, e a distância entre os
> dois é o trabalho que falta.

⚠️ **Só dois palcos têm grade horária montada** — e quase tudo nela ainda está *a confirmar*.
