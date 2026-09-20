# Cadência — sprints semanais (em 2026, de terça a terça)

> A régua de prazo do FING 2026. Quem lê: o agente `radar-de-prazos` e qualquer pessoa
> que anote item nos arquivos de pendência desta pasta.
>
> Definida pelo Lucas em **03/09/2026**. Vale até o evento.

## A regra

**Prazo acordado por item = 7 dias = 1 sprint.** A sprint começa e termina no **dia da
reunião semanal da coordenação**, que é o único momento em que prazo se pactua ou se
repactua — de uma reunião à outra, prazo não muda sozinho.

> 📅 **O ciclo semanal é a regra; o dia da semana, não.** Em **2026 a coordenação escolheu
> a terça-feira**, por ter sido o melhor dia para todos os coordenadores desta edição. Cada
> edição escolhe o seu — ao mudar de edição, troque o dia aqui e siga com o resto igual.

Item levantado no meio da sprint **entra na sprint seguinte**, porque é na reunião que ele é
assumido por alguém. Puxar item para a sprint corrente é possível, mas é decisão da reunião,
não do agente nem de quem anotou.

## Como escrever o prazo num item

Um campo só, dentro do `<sub>` que o item já tem:

```markdown
- [ ] **O item.** Descrição.
      <sub>Prazo: 15/09 (S02) · Origem: `CLAUDE.md` §6 · 02/09/2026</sub>
```

- **`Prazo:`** vem primeiro — é o que se lê de relance.
- **Origem e data** continuam sendo a data em que o item foi **levantado**, não o prazo.
  São coisas diferentes e a confusão entre as duas é o que fazia o radar rodar cego.

### Item que rola de sprint

Não saiu na sprint, a reunião repactua e o contador de rolagem sobe:

```markdown
      <sub>Prazo: 22/09 (S03, 2ª rolagem) · Origem: ...</sub>
```

O contador é o dado que interessa. Um item na **3ª rolagem** não é um item atrasado — é um
item que a coordenação vem assumindo sem conseguir entregar, e isso é pauta da reunião:
ou muda o dono, ou muda o escopo, ou sai da lista.

### Item na mão de terceiro

Sesc, Sebrae, patrocinadores, plataforma de inscrição, contador — não respondem a cobrança
interna. Para esses, **o prazo
da sprint é do follow-up, não da entrega**: o que vence na reunião é ter feito o contato, não
ter recebido a resposta. Marcar assim:

```markdown
      <sub>Prazo: 15/09 (S02, follow-up) · Origem: ...</sub>
```

Assim um item parado em terceiro por seis semanas mostra seis follow-ups, e não seis atrasos
de quem não podia entregar.

## Calendário até o evento

| Sprint | Início (ter) | Fim (ter) | |
|---|---|---|---|
| S01 | 01/09 | 08/09 | sprint em que a cadência foi criada |
| S02 | 08/09 | 15/09 | |
| S03 | 15/09 | 22/09 | |
| S04 | 22/09 | 29/09 | |
| S05 | 29/09 | 06/10 | |
| S06 | 06/10 | 13/10 | |
| S07 | 13/10 | 20/10 | |
| S08 | 20/10 | 27/10 | |
| S09 | 27/10 | 03/11 | |
| S10 | 03/11 | 10/11 | |
| S11 | 10/11 | 17/11 | |
| S12 | 17/11 | 24/11 | **última sprint inteira antes do evento** |
| S13 | 24/11 | 01/12 | montagem 27/11 · **evento 28/11** · desmontagem 29/11 |

São **11 sprints de trabalho** entre a reunião de 08/09 e a de 24/11. Depois disso o que não
estiver pronto não fica pronto.

## O que isso destrava

O `radar-de-prazos` foi escrito para cruzar dependência **e** prazo, mas rodou sem a segunda
metade porque o `todo/` só guardava data de levantamento. Com o campo `Prazo:`, ele passa a
distinguir três coisas que antes eram uma só: o que está **atrasado**, o que **vence nesta
sprint** e o que apenas **está aberto**.
