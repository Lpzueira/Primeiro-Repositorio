---
name: atendimento-faq
description: Perguntas frequentes e respostas do primeiro atendimento da Casa em Conta (WhatsApp Business e direct do Instagram), regras de quando passar para o dono e plano do atendimento automático. Use para responder alguém, revisar as respostas rápidas ou montar o robô de atendimento no futuro.
---

# Atendimento: Casa em Conta

Os textos prontos para configurar no app (saudação, ausência e respostas rápidas) estão em `divulgacao/whatsapp-business-respostas.md`. Esta skill traz as respostas e as regras.

## Regras

- Curto, simpático, "estou/está". Responda o que foi perguntado e, se fizer sentido, ofereça o grupo ou a vitrine.
- A Casa em Conta **não vende nada**: indica produtos do Mercado Livre. Pedido, pagamento, entrega, troca, devolução e garantia são com o **Mercado Livre**.
- **Nunca** peça CPF, senha, código de verificação, dados de cartão ou endereço. Se a pessoa mandar, avise para apagar e não mandar a ninguém.
- Não prometa preço, estoque, prazo ou reembolso.

## Perguntas frequentes

| Pergunta | Resposta |
|---|---|
| Como entro no grupo? | Pelo link da bio do Instagram ou direto: https://lpzueira.github.io/casaemconta/ (é grátis e só eu posto). |
| O grupo é pago? | Não, é grátis. Eu ganho uma pequena comissão do Mercado Livre quando alguém compra por um link meu, sem custo extra para você. |
| Vocês vendem o produto? | Não. Eu só indico achadinhos; a compra é feita direto no Mercado Livre, com a garantia e a entrega deles. |
| O preço mudou / o desconto acabou | Os preços são do Mercado Livre e mudam rápido, às vezes em minutos. Eu posto o preço que vi na hora. |
| Meu pedido não chegou / veio com defeito | Isso é resolvido direto no Mercado Livre: em "Minhas compras", abra a compra e toque em "Preciso de ajuda". |
| Tem cupom? | Quando aparece cupom bom, eu mando no grupo. Fica de olho nos 3 horários do dia. |
| Pode procurar um produto para mim? | Quando dá, sim! Me conta o que você procura e a faixa de preço. (Passe para o dono.) |
| Quero sair do grupo / parar de receber | É só sair do grupo nas informações do grupo. Se preferir, silencie e olhe quando quiser. |
| É golpe? | Não pedimos dados nem pagamento. Todos os links levam ao site oficial do Mercado Livre, e o perfil está no Instagram @casa.emconta01. |
| Quero fazer parceria / publicidade | Passe para o dono. |

## Passar para o dono quando

Reclamação séria ou ofensa, problema com pedido que a resposta padrão não resolveu, parceria/publicidade/imprensa, pedido sobre dados pessoais (LGPD), pedido de produto específico, ou qualquer dúvida fora desta lista.

## Plano do atendimento automático

- **Agora (grátis):** mensagens de saudação e de ausência e respostas rápidas do WhatsApp Business, com os textos de `divulgacao/whatsapp-business-respostas.md`.
- **Fase 3:** atendente automático oficial (API do WhatsApp num número próprio, ou ManyChat no direct do Instagram) usando esta FAQ, sempre com a opção de falar com o dono. Ferramentas não oficiais que automatizam o WhatsApp **não** devem ser usadas: risco de banir o número que administra o grupo.
- Robô **dentro do grupo** não é possível de forma oficial (a API oficial de grupos aceita no máximo 8 participantes).
