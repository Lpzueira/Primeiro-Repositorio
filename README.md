# Casa em Conta: página de captura

No ar em: https://lpzueira.github.io/casaemconta/

Página "link na bio" do Instagram [@casa.emconta01](https://www.instagram.com/casa.emconta01/), que leva o visitante para o grupo VIP de achadinhos no WhatsApp.

## Arquivos

- `index.html`: a página inteira (HTML, CSS e JS num arquivo só).
- `assets/`: logo, ícone da aba e fotos da obra usadas na página.

Cada botão tem um `data-cta` (`hero`, `fixo`, `final`, `topo-instagram`, `topo-vitrine`, `final-instagram`, `final-vitrine`, `album-instagram`) para medir cliques quando o Pixel da Meta for instalado.

## Como editar os links

No final do `index.html` existe um bloco `CONFIG`:

```js
const CONFIG = {
  whatsapp: "https://chat.whatsapp.com/...",  // convite do grupo
  instagram: "https://www.instagram.com/casa.emconta01/",
  vitrine: "https://meli.la/2BbXAdh"           // vitrine de afiliado no Mercado Livre
};
```

Quando o grupo chegar perto de 1.024 membros (o limite do WhatsApp), crie o grupo 2 e troque o link `whatsapp`. Todos os botões da página passam a apontar para o grupo novo.

## Como publicar (grátis)

O repositório é **privado**, e o GitHub Pages só funciona de graça em repositório **público**. Há duas opções:

1. **GitHub Pages:** torne o repositório público (*Settings → General → Danger Zone → Change visibility*). Depois, em *Settings → Pages*, escolha *Deploy from a branch*, a branch `main` e a pasta `/ (root)`. O endereço fica `https://lpzueira.github.io/casaemconta/`.
2. **Netlify ou Cloudflare Pages:** conecte o repositório privado ou arraste o `index.html`. Também é grátis.

Depois de publicar, coloque o endereço na bio do Instagram.

## Checklist do grupo no WhatsApp

- Em *Configurações do grupo*, ative **Enviar mensagens: somente admins**, como a página promete.
- Coloque na descrição do grupo o aviso de afiliado e as regras.
- Fixe uma mensagem de boas-vindas.

## Domínio próprio (próximo passo)

Quando os resultados começarem, registre `casaemconta.com.br` no registro.br (cerca de R$ 40 por ano) e aponte para o GitHub Pages em *Settings → Pages → Custom domain*. O link `lpzueira.github.io/casaemconta` continua funcionando e redireciona para o domínio.
