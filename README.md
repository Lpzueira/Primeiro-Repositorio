# Casa em Conta: página de captura

No ar em: https://lpzueira.github.io/casaemconta/

Página "link na bio" do Instagram [@casa.emconta01](https://www.instagram.com/casa.emconta01/), que leva o visitante para o grupo VIP de achadinhos no WhatsApp.

## Arquivos

- `index.html`: a página inteira (HTML, CSS e JS num arquivo só).
- `privacidade.html`: Política de Privacidade (Pixel da Meta, LGPD e contato pelo direct do Instagram), com link no rodapé da página.
- `assets/`: logo, ícone da aba e fotos da obra usadas nas páginas.
- `divulgacao/`: textos de anúncios e do grupo, capa e foto de perfil do Facebook. **Não** é publicada no site.
- `_config.yml`: diz ao GitHub Pages para **não** publicar no site o `CLAUDE.md`, o `README.md` e a pasta `divulgacao/`.
- `CLAUDE.md` e `.claude/`: instruções para o Claude, a equipe de agentes (`.claude/agents/`), as skills (`.claude/skills/`) e a trava de segurança (`.claude/settings.json`), que pede confirmação antes de qualquer ação que mexa nos anúncios.
- `divulgacao/rotina-no-pc.md`: como postar pelo PC; `divulgacao/whatsapp-business-respostas.md`: respostas automáticas e rápidas do WhatsApp Business.

Cada botão tem um `data-cta` (`hero`, `fixo`, `final`, `topo-instagram`, `topo-vitrine`, `final-instagram`, `final-vitrine`, `album-instagram`, `faixa-black-friday`), que vai no parâmetro `origem` dos eventos do Pixel.

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

## Repositório público e publicação

- Este repositório é **público** (o GitHub Pages grátis exige isso). Por isso, **nunca** grave aqui senhas, chaves, IDs de contas de anúncios, dados de pagamento, gastos ou histórico da campanha. Esses dados ficam num repositório **privado** separado.
- O histórico do Git guarda todas as versões antigas dos arquivos: o que já foi publicado deve ser tratado como público.
- O site é publicado pelo **GitHub Pages a partir da branch `main`**, pasta `/ (root)` (*Settings → Pages*). Qualquer merge na `main` atualiza o site em cerca de 1 minuto.
- Como a campanha leva tráfego para a página, toda mudança no site segue: preparar numa branch → testar no celular e no computador → aprovação do dono → merge na `main` → conferir o site no ar.

## Checklist do grupo no WhatsApp

- Em *Configurações do grupo*, ative **Enviar mensagens: somente admins**, como a página promete.
- Coloque na descrição do grupo o aviso de afiliado e as regras.
- Fixe uma mensagem de boas-vindas.

## Domínio próprio (próximo passo)

Quando os resultados começarem, registre `casaemconta.com.br` no registro.br (cerca de R$ 40 por ano) e aponte para o GitHub Pages em *Settings → Pages → Custom domain*. O link `lpzueira.github.io/casaemconta` continua funcionando e redireciona para o domínio.

## Meta Pixel

Pixel `1477454040680046` (portfólio Casa em Conta), instalado no `<head>` do `index.html`.

| Evento | Quando dispara |
|---|---|
| `PageView` | Ao abrir a página |
| `Lead` | Clique em qualquer botão do grupo do WhatsApp (conversão das campanhas) |
| `CliqueInstagram` | Clique em botões do Instagram |
| `CliqueVitrine` | Clique no botão da vitrine do Mercado Livre |

Cada evento leva o parâmetro `origem` com o `data-cta` do botão clicado.
