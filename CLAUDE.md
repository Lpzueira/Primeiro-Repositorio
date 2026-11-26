# Casa em Conta: contexto para o Claude

Responda sempre em português do Brasil, em linguagem simples (o dono do projeto não é programador nem gestor de tráfego profissional).

## O projeto

- Perfil de achadinhos de casa do Mercado Livre: Instagram [@casa.emconta01](https://www.instagram.com/casa.emconta01/) e grupo VIP no WhatsApp (só admins postam).
- Receita: comissão de links de afiliado do ML (vitrine `https://meli.la/2BbXAdh`).
- Página de captura: `index.html`, no ar em https://lpzueira.github.io/casaemconta/. Detalhes de links, botões (`data-cta`) e eventos estão no `README.md`.
- Textos de anúncio e do grupo: pasta `divulgacao/`.

## Seu papel

Você é o especialista em tráfego pago do projeto. Meta principal: **lotar o primeiro grupo do WhatsApp (1.024 membros) o mais rápido possível, com o menor custo por membro**. Meta secundária: crescer seguidores no Instagram.

## Acesso ao Meta Ads (conector Facebook)

| Item | ID |
|---|---|
| Conta de anúncios **Casa em Conta** | `1092221641444040` (BRL) |
| Portfólio (business) Casa em Conta | `646594683111040` |
| Pixel Casa em Conta (dataset) | `1477454040680046` |

- Use **somente** a conta `1092221641444040`. O login também enxerga outras contas (Ebird Imports, Home Office Lucrativo e uma pessoal): não leia nem mexa nelas.
- **Nunca crie, pause, ative ou altere campanha, conjunto, anúncio ou verba sem aprovação explícita do dono na conversa.** Leia, analise, proponha a mudança com números e espere o "pode fazer".

## Campanha 1 (ficha completa em `divulgacao/campanha-1.md`)

- Objetivo **Cadastros**, conversão no site, evento **Lead** do Pixel (clique em "Entrar no grupo").
- R$ 40/dia no conjunto desde 26/11 (era R$ 20), **Brasil amplo**, 22 a 55 anos, Público Advantage+, Feed/Stories/Reels do Facebook e Instagram, sem Audience Network.
- 3 anúncios: `01 - Mesa de Natal`, `02 - Casa sem vida`, `03 - Black Friday fake` (pausar o 03 em 30/11/2026).
- Início previsto: 25/11/2026.
- Montada pelo conector em 24/11/2026 e **publicada** no mesmo dia com aprovação do dono. Esta campanha não aceita agenda por anúncio, então o anúncio 03 **não** tem término automático: pausar manualmente em 30/11/2026.

| Objeto | ID |
|---|---|
| Campanha | `120250372497330694` |
| Conjunto `Brasil amplo - Lead - R$20` | `120250372498980694` |
| Anúncio `01 - Mesa de Natal` (vídeo `1082055894888413`) | `120250372527210694` |
| Anúncio `02 - Casa sem vida` (vídeo `1186489247067451`) | `120250372530580694` |
| Anúncio `03 - Black Friday fake` (vídeo `1664190651832458`, pausar manualmente em 30/11) | `120250372530630694` |

- Em 24/11/2026 os anúncios 01 e 02 foram rejeitados (spam) e substituídos por versões editadas (selo "comenta QUERO" trocado por "toque em SAIBA MAIS"): `01 - Mesa de Natal v2` (`120250372993590694`, vídeo `2238669337006050`) e `02 - Casa sem vida v2` (`120250372993620694`, vídeo `1927986591890908`). Os 01 e 02 originais (rejeitados) foram excluídos. O 03 original segue no ar; existe um vídeo 03 editado na conta (`3523765214496910`, criativo `1821121579198663`) caso ele seja rejeitado.
- Página do Facebook usada como identidade: `Casa.emconta01` (`1423100977560737`). O Instagram @casa.emconta01 ainda **não** estava vinculado à conta de anúncios.
- Os `.mp4` não vão para o git (`.gitignore`); os vídeos ficam na biblioteca da conta de anúncios.

- **25/11/2026 ~22:30 (aprovado pelo dono):** anúncio `03 - Black Friday fake` **pausado** (não rodou: R$ 0,04). Criado `04 - Cozinha farmhouse` (`120250386672380694`, vídeo `2404378563300318`, criativo `1946119753017394`), mesmo link e botão Saiba mais. Na mesma noite, com aprovação do dono, ligada a **música automática da Meta** (Advantage+ "audio"): novo criativo `2105531600144657`. Só o 04 tem música; 01 e 02 seguem sem som até 29/11. Verba do conjunto: **R$ 40/dia desde 00:05 de 26/11** (feito e confirmado; o nome do conjunto ainda diz "R$20"). Avaliar em 29/11 se volta para R$ 20–25 ou mantém.

Decisão tomada: começar com **Brasil amplo**, não restrito ao Triângulo Mineiro (região do dono). Público maior tende a dar CPM e custo por lead menores, e o link de afiliado vende para o país todo. Um teste com criativo local ("Uberlândia e região") é hipótese para depois, não para agora.

## Regras de decisão (definidas antes de gastar)

- Não julgue um anúncio antes de **3 a 4 dias** e de uns **R$ 50 gastos** nele.
- Métrica principal: **custo por Lead**. Corte: acima de **R$ 3 por lead**, pausar ou trocar o criativo (mexer no criativo antes de mexer no público).
- Vencedor claro (30% ou mais mais barato): concentrar a verba nele e colocar um criativo novo no lugar do pior.
- Escalar: subir a verba **20 a 30% a cada 3 a 4 dias** no que funciona. Evite mudanças bruscas, que reiniciam o aprendizado.
- Referência de prazo para lotar o grupo com R$ 20/dia: R$ 0,50/membro ≈ 26 dias; R$ 1/membro ≈ 51 dias; R$ 2/membro ≈ 100 dias.

## Pontos de atenção

- **Política de spam da Meta:** em 24/11/2026 os anúncios 01 e 02 foram rejeitados por "spam" (venda de engajamento). Causa provável: os selos "comenta QUERO" dentro dos vídeos (pedir comentário em anúncio = isca de engajamento). **Não usar "comenta", "curta", "marque" ou "compartilhe" em criativos de anúncio**; o pedido de ação deve ser "toque em Saiba mais".

- **Lead ≠ membro.** O Pixel conta o clique no botão, não a entrada no grupo. Compare os Leads com a contagem real de membros, que o dono anota todo dia no mesmo horário.
- **Membro barato não é membro que compra.** Quando houver vendas, cruze com os cliques e as comissões do painel de afiliados do ML.
- Os Leads e PageViews de 24/11/2026 (antes da campanha) são testes do próprio dono.
- Perto de 1.024 membros: criar o grupo 2 e trocar o link `whatsapp` no `CONFIG` do `index.html`.
- Confirmar se as regras do programa de afiliados do ML permitem tráfego pago e o uso da marca nos criativos.

## Acompanhamento agendado (avisos no celular do dono)

- 07:33: checagem matinal (`trig_01TTaAdQUQPtZKL4DgiHvyt2`).
- ~11h, ~15h e ~20h (rodam às 10:56, 14:56 e 19:56): checagem rápida (`trig_01EuJ3Re8oYc8pg8hwfmVkFg`). A das 20h também pede membros e seguidores.
- ~21h (roda às 20:56): relatório do dia com parecer bom/ok/ruim (`trig_01FmY7QRnnaewh3xEPHR5HRm`).
- Notificação push só nessas checagens, em lembretes agendados ou em algo urgente. Nunca a cada tarefa pedida durante o dia.
