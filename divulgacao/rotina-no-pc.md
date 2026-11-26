# Rotina de postagem pelo PC

Como usar o grupo e a equipe do Claude pelo computador, sem depender do celular onde está o WhatsApp Business.

## 1. WhatsApp Business no PC (oficial)

1. No PC, abra o **WhatsApp** (app para Windows/Mac) ou https://web.whatsapp.com.
2. No celular do WhatsApp Business: *Configurações → Dispositivos conectados → Conectar dispositivo* e escaneie o QR code da tela do PC.
3. Pronto: o grupo e as conversas aparecem no PC. O celular não precisa ficar ao lado; só precisa entrar na internet de vez em quando (o WhatsApp desconecta os aparelhos se o celular ficar uns 14 dias sem abrir).

É o próprio recurso do WhatsApp, sem risco para o número.

## 2. Claude no PC, com o repositório

O repositório não "segura" uma conexão com o WhatsApp: ele guarda as instruções, a equipe de especialistas e os textos. O Claude trabalha no PC lendo o repositório:

1. Use o Claude Code no PC com os repositórios `Lpzueira/casaemconta` e `Lpzueira/casaemconta-privado`.
2. Para escolher produtos, o Claude precisa ver o Mercado Livre: no PC isso funciona com o navegador (Claude no Chrome) e a sua conta do ML logada. Na nuvem, o ML bloqueia as páginas de produto.
3. Peça, por exemplo: **"prepara o lote de posts de amanhã, tema do calendário"**. O `curador-de-ofertas` escolhe os produtos, você gera (ou confere) o link de afiliado na barra do ML, e o `redator-de-posts` entrega os 3 posts prontos.
4. Os lotes ficam guardados no repositório privado, em `posts/AAAA-MM-DD.md`.

## 3. Postar

Nos 3 horários, copie o post do lote e cole no grupo pelo WhatsApp do PC. Leva uns 30 segundos por post.

## O que não fazer

- **Não** use robôs, extensões de "disparo" ou serviços que automatizam o WhatsApp (Z-API, Evolution e parecidos), nem deixe um programa clicar em "enviar" por você. Isso quebra as regras do WhatsApp e pode **banir o número que administra o grupo**, e o grupo se perde junto.
- **Não** passe senha, código de verificação ou o QR code do WhatsApp para ninguém (nem para o Claude).
