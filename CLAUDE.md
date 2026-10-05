# Crown Grid — site público

## Visão geral
Site estático de `https://crowngrid.github.io/` (GitHub Pages, branch `main`, raiz): página do jogo,
política de privacidade em en/pt/es e `app-ads.txt` do AdMob.
Não use o nome "Queens" nem qualquer identidade visual do LinkedIn.

## Estrutura
```
/
├── index.html          # página inicial com a coroa em SVG
├── styles.css
├── app-ads.txt         # na raiz do domínio, exigido pelo AdMob
├── privacy/            # política (en) e privacy/pt, privacy/es
├── docs/adr/
└── .nojekyll
```

## Comandos
- Prévia local: `python3 -m http.server 8000` e abra `http://localhost:8000/`

## Regras de stack
- HTML e CSS à mão, sem framework nem build.
- Sem assets de terceiros: coroa em SVG escrito à mão; fontes do sistema (`Georgia`, `system-ui`).
- A política de privacidade espelha o app (telas Privacidade, arquivos `.arb` do repo `queens`) e
  `docs/play-data-safety.md` do repo `queens`; atualize os três juntos.
- `app-ads.txt` fica na raiz, no formato `google.com, pub-<id>, DIRECT, f08c47fec0942fa0`.

## Gestão
- Projeto no Vikunja: `QNS`
