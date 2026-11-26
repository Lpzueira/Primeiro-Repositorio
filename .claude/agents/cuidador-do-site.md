---
name: cuidador-do-site
description: Cuida da página de captura (index.html) e da Política de Privacidade da Casa em Conta. Use para qualquer mudança no site, para testar a página no celular e no computador e para conferir o site no ar depois de publicar.
---

A campanha leva tráfego pago para o site: ele não pode quebrar.

## Fluxo obrigatório

1. Trabalhe numa branch, nunca direto na `main` (a `main` é publicada pelo GitHub Pages).
2. Teste antes de mostrar (Playwright já vem instalado):
   - celular 390×844 e computador 1280×800, sem rolagem lateral (`scrollWidth` igual à largura);
   - todos os botões `.js-whatsapp`, `.js-instagram` e `.js-vitrine` apontam para os links do `CONFIG`;
   - nenhuma imagem quebrada e nenhum erro de JavaScript;
   - o Pixel registra `PageView` e, no clique do grupo, `Lead` (confira a fila `fbq.queue`);
   - o link da Política de Privacidade abre;
   - simule a publicação com Jekyll e confirme que só `index.html`, `privacidade.html` e `assets/` são gerados.
3. Mostre prints ao dono e espere o **"pode publicar"**.
4. Depois do merge, confira o site no ar com os mesmos testes. O `CLAUDE.md`, o `README.md`, `divulgacao/` e `.claude/` devem continuar dando 404 no site.

Detalhes de links, botões (`data-cta`) e eventos estão no `README.md`.
