# Manual do usuário — Bússola Premiada

Site Jekyll (tema [just-the-docs](https://just-the-docs.com/)) do manual público do
**Bússola Premiada**, publicado em <https://docs.bussola-premiada.rit.org.br>.

## Estrutura

- `index.md` — página inicial.
- `primeiros-passos.md`, `papeis.md` — orientação inicial.
- `guias/` — guias por tarefa (passo a passo).
- `modulos/` — referência por módulo do plugin.
- `boas-praticas/` — campanhas vencedoras, prêmios, divulgação, requisitos legais.
- `faq.md`, `novidades.md` — dúvidas frequentes e changelog para leigos.
- `legal/` — aviso, privacidade, termos e licença (GPL).
- `assets/` — logo, favicon e `screenshots/` (capturas de tela).

## Publicação

Este diretório é a **fonte**. A publicação é feita a partir do repositório do plugin
com:

```bash
bin/publish-manual.sh          # espelha docs-publico/ -> RIT-DF/docs-bussola-premiada -> Pages
bin/publish-manual.sh -n       # dry-run
```

O GitHub Actions do repositório do manual builda o Jekyll e publica no GitHub Pages.

## Rodar localmente

```bash
cd docs-publico
bundle install
bundle exec jekyll serve
```

## Manutenção

Depois do bootstrap (skill `user-manual`), a manutenção incremental é da skill
`docs-keeper`. Cada página tem uma front-matter com `routes`/`screenshots` que permite
saber o que uma mudança de código afeta. Capturas são recriadas pela skill `user-manual`.
