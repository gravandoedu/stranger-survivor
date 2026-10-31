# Stranger Survivor Publisher — site do app do TikTok

Páginas estáticas para usar nos campos **Web URL**, **Terms of Service URL** e
**Privacy Policy URL** do app no TikTok for Developers.

> Modelo simples de termos e privacidade. Não é aconselhamento jurídico. Se
> precisar, revise com um advogado.

## URLs

Com o GitHub Pages publicado na branch `main`, pasta `/`:

- Web URL: `https://gravandoedu.github.io/stranger-survivor/`
- Termos de Uso: `https://gravandoedu.github.io/stranger-survivor/termos.html`
- Política de Privacidade: `https://gravandoedu.github.io/stranger-survivor/privacidade.html`
- Redirect URI do OAuth: `https://gravandoedu.github.io/stranger-survivor/callback.html`

Versões em inglês: `terms.html` e `privacy.html`.

## Publicar

1. No GitHub, abra **Settings → Pages**.
2. Em **Source**, escolha **Deploy from a branch**.
3. Selecione a branch `main` e a pasta `/ (root)`.
4. Salve e espere o GitHub mostrar o endereço do site.

## Usar no TikTok

No cadastro do app, preencha:

- **Description**: a frase curta do `index.html`.
- **Web URL**: a URL do `index.html`.
- **Terms of Service URL**: a URL do `termos.html`.
- **Privacy Policy URL**: a URL do `privacidade.html`.
- **Redirect URI**: a URL do `callback.html`.

A Redirect URI também precisa ir para `redes.tiktok.redirect_uri` no
`config/settings.yaml`, exatamente igual. O `callback.html` não faz login; ele só
mostra a URL final para você copiar e colar no `tiktok-login`.

## Contato

O email usado nas páginas é `gravandoedu@users.noreply.github.com`. Troque por um
email que você realmente lê antes de enviar o app para revisão do TikTok.
