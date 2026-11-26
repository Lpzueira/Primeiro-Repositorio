---
name: trafego-pago
description: Regras de decisão e rotina das checagens dos anúncios da Casa em Conta no Meta Ads. Use sempre que for analisar a campanha, rodar uma checagem agendada (matinal, rápida ou relatório das 21h), dar parecer bom/ok/ruim, calcular custo por lead ou por membro, ou propor pausar, trocar criativo ou mudar a verba.
---

# Tráfego pago: Casa em Conta

Antes de começar: leia o `CLAUDE.md` deste repositório (papel, metas, regra de aprovação, pontos de atenção) e o `CLAUDE.md` do repositório privado `Lpzueira/casaemconta-privado` (IDs da conta e da campanha, situação atual, pagamento). Se o repositório privado não estiver na sessão, adicione-o.

**Regra de ouro:** nunca crie, pause, ative ou altere campanha, conjunto, anúncio ou verba sem o "pode fazer" do dono na conversa. Leia, analise e **proponha com números**. A trava em `.claude/settings.json` também pede confirmação antes dessas ações.

## Regras de decisão (definidas antes de gastar)

- Não julgue um anúncio antes de **3 a 4 dias** e de uns **R$ 50 gastos** nele.
- Métrica principal: **custo por Lead**. Corte: acima de **R$ 3 por lead**, pausar ou trocar o criativo (mexer no criativo antes de mexer no público).
- Vencedor claro (30% ou mais mais barato): concentrar a verba nele e colocar um criativo novo no lugar do pior.
- Escalar: subir a verba **20 a 30% a cada 3 a 4 dias** no que funciona. Evite mudanças bruscas, que reiniciam o aprendizado.
- Referência de prazo para lotar o grupo com R$ 20/dia: R$ 0,50/membro ≈ 26 dias; R$ 1/membro ≈ 51 dias; R$ 2/membro ≈ 100 dias.
- Regras do programa de afiliados do ML (tráfego pago e uso da marca nos criativos): o dono decidiu **conferir quando a campanha estiver dando resultados** (vendas ou comissões aparecendo). Quando isso acontecer, lembre o dono.

Decisão tomada: começar com **Brasil amplo**, não restrito ao Triângulo Mineiro (região do dono). Público maior tende a dar CPM e custo por lead menores, e o link de afiliado vende para o país todo. Um teste com criativo local ("Uberlândia e região") é hipótese para depois, não para agora.

## Como medir

- **Lead ≠ membro.** O Pixel conta o clique no botão do WhatsApp, não a entrada no grupo. O custo real sai da contagem de membros que o dono informa.
- **Custo por membro** = gasto acumulado ÷ (membros hoje − membros no ponto de partida). Tabela e ponto de partida em `divulgacao/acompanhamento.md` do repositório **privado**.
- **Membro barato não é membro que compra.** Quando houver vendas, cruze com os cliques e as comissões do painel de afiliados do ML.

## Rotina das checagens agendadas

Todas usam o conector do Facebook, **só** na conta e na campanha indicadas no `CLAUDE.md` privado. Dados, gastos e histórico são gravados **só no repositório privado**, nunca no público.

### Checagem matinal (07:33)

1. Status de cada anúncio (aprovado/reprovado/ativo/pausado) e métricas de **ontem** e do **acumulado desde 25/11**, por anúncio e no total: valor gasto, resultados (Lead), custo por lead, CTR do link, CPM e frequência.
2. Comparar com as regras de decisão acima. Se houver algo a fazer, propor com números, sem alterar nada.
3. Lembretes da manhã do `CLAUDE.md` privado (pagamento e saldo). Pedir o número de membros do grupo e de seguidores do Instagram para atualizar `divulgacao/acompanhamento.md` do repositório privado.
4. Formato: português simples, curto (no máximo uns 10 itens), com uma tabela por anúncio.

### Checagem rápida (10:56, 14:56 e 19:56)

1. Status de cada anúncio e métricas de **hoje** por anúncio e no total: valor gasto, leads, custo por lead, CTR do link e CPM.
2. Só propor mudança se houver algo fora do normal: anúncio rejeitado, custo por lead acima de ~R$ 5 no dia, entrega parada.
3. Formato: bem curto (tabela por anúncio + 2 ou 3 frases). Na das 20h, pedir também membros do grupo e seguidores do Instagram.

### Relatório das 21h (20:56)

1. Métricas de **hoje** e do **acumulado desde 25/11**, por anúncio e no total: valor gasto, leads, custo por lead, cliques no link, CTR do link, CPM, alcance e frequência. Status de cada anúncio.
2. Se o dono informou o número de membros hoje, calcular o custo real por membro e atualizar `divulgacao/acompanhamento.md` do repositório privado. Se houve mudança na campanha, registrar em `divulgacao/historico-campanha.md` do repositório privado.
3. **Parecer claro: BOM, OK ou RUIM**, comparando com as regras de decisão e com os dias anteriores, e dizer o que esperar para amanhã. Se houver algo a mudar, propor com números.
4. Formato: tabela + parecer em poucas linhas.

### Parecer bom/ok/ruim (critérios aprovados pelo dono em 26/11/2026)

- **BOM:** custo por lead dentro do corte (até R$ 3) e custo por membro caindo ou estável; nenhum anúncio rejeitado.
- **OK:** custo dentro do corte mas subindo, ou poucos dados para julgar (antes de 3 a 4 dias ou de ~R$ 50 por anúncio).
- **RUIM:** custo por lead acima do corte, anúncio rejeitado, entrega parada ou saldo perto de zerar.

## Notificações

- Toda checagem termina com uma **notificação push curta** (menos de 200 caracteres) para o celular do dono: gasto, leads, custo por lead e se algo precisa de atenção. No relatório das 21h, incluir o parecer (bom/ok/ruim).
- Push só nessas checagens, em lembretes agendados ou em algo urgente. Nunca a cada tarefa pedida durante o dia.
- Mudanças agendadas que mexem em dinheiro (verba, ativar/pausar) pedem confirmação do dono no app na hora de executar. Agende-as entre 7h e 22h, nunca de madrugada.

## Criativos

- **Política de spam da Meta:** não usar "comenta", "curta", "marque" ou "compartilhe" em criativos de anúncio. O pedido de ação é "toque em Saiba mais". (Em 24/11/2026 dois anúncios foram rejeitados por causa do selo "comenta QUERO".)
