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

O Pages está publicado pela branch `gh-pages`. Para atualizar o site:

1. Faça as mudanças na branch `main` e envie.
2. Sincronize a `gh-pages` e envie:

```bash
git checkout gh-pages
git merge main --ff-only
git push origin gh-pages
git checkout main
```

3. O GitHub reconstrói o site sozinho.

Se a `gh-pages` não avançar por fast-forward:

```bash
git branch -f gh-pages main
git push origin gh-pages --force
```

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

O email usado nas páginas é `gravandoedu@gmail.com`.
