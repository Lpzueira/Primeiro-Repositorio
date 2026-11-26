---
name: relatorio-semanal
description: Monta o relatório semanal de resultados da Casa em Conta (anúncios, membros do grupo, seguidores e comissões do Mercado Livre), com parecer e plano da semana seguinte. Use todo domingo à noite ou quando o dono perguntar como o projeto está indo.
---

# Relatório semanal: Casa em Conta

## De onde vêm os números

| Dado | Fonte |
|---|---|
| Gasto, leads, custo por lead, CTR, CPM por anúncio | Conector do Facebook (só leitura), conta e campanha do `CLAUDE.md` privado |
| Membros do grupo e seguidores | `divulgacao/acompanhamento.md` do repositório **privado** (o dono informa) |
| Cliques, vendas e comissões do ML | **Print do painel de afiliados** enviado pelo dono (não há API oficial) |
| Posts da semana | Lotes preparados pelo `redator-de-posts` |

Se faltar algum dado, diga qual e peça ao dono. Nunca invente números.

## Formato

1. **Resumo em 3 linhas:** a semana foi BOA, OK ou RUIM e por quê (critérios da skill `trafego-pago`).
2. **Tabela da semana:** gasto, leads, custo por lead, novos membros, custo por membro, seguidores novos, cliques no ML, vendas, comissão.
3. **Comparação com a semana anterior** (setas ↑ ↓ e %).
4. **O que funcionou:** melhor anúncio, melhor horário e melhor tipo de post (se o painel do ML mostrar cliques por link).
5. **Plano da próxima semana:** tema (skill `calendario-de-ofertas`), mudanças propostas nos anúncios **com números** (só com o "pode fazer" do dono) e um teste novo.
6. **Lembretes:** saldo da conta de anúncios, regras do programa de afiliados quando houver vendas, mensagem fixada do período.

## Onde gravar

Só no repositório **privado**: `relatorios/AAAA-MM-DD-semana.md`. Nunca no repositório público.
