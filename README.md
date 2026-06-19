# Berry Design System

Sistema de design oficial da **Berry Consultoria**: o sistema visual e verbal derivado do manual de identidade e dos arquivos oficiais da marca.

O repositório se organiza em duas camadas que trabalham juntas:

- **`index.html`** é o showcase. Abre direto no navegador, sem build, e renderiza o sistema inteiro com modo escuro e claro. Ele agora consome os arquivos modulares (`tokens/`, `styles/`, `components/`) via `<link>`, então não há CSS duplicado: o que se vê no showcase é exatamente o código-fonte das pastas.
- **As pastas** (`tokens/`, `foundations/`, `components/`, `assets/`) são a fonte modular e documentada, organizada no padrão de mercado: uma camada de tokens como fonte única de verdade, fundamentos documentados, um componente por pasta e os vetores oficiais como arquivos.

## Estrutura

```
system-design-berry/
├── index.html                  # showcase; consome tokens/ styles/ components/ via <link>
├── tokens/                     # fonte única de verdade
│   ├── tokens.json             # formato W3C Design Tokens (DTCG)
│   ├── tokens.css              # espelho em CSS custom properties + tema claro
│   └── README.md
├── foundations/                # fundamentos documentados (o porquê e o como)
│   ├── brand/  color/  typography/  layout/
│   └── surfaces/  motion/  iconography/  logo/
├── components/                 # um componente por pasta
│   └── <componente>/
│       ├── <componente>.css    # estilos (extraídos com fidelidade do fonte)
│       ├── <componente>.html   # preview isolado, abre no navegador
│       └── README.md           # classes, variações, tokens, uso
├── assets/
│   ├── logo/                   # 6 lockups oficiais em SVG
│   └── icons/                  # 15 glifos em SVG de traço
└── styles/                     # reset, base, layout e showcase compartilhados
```

## Componentes

`theme-toggle` · `button` · `input` · `card` · `badge` · `tag` · `pill` · `stat` · `testimonial` · `trust-seal` · `list` · `divider` · `icon-badge`

Cada pasta traz o CSS do componente, um preview que abre sozinho no navegador e um README com classes, variações e tokens. Os previews carregam `tokens/tokens.css` e `styles/`, provando que cada componente funciona de forma isolada.

## Como usar

**Ver o sistema inteiro:** abra `index.html`.

**Ver um componente isolado:** abra, por exemplo, `components/button/button.html`.

**Consumir em um produto:** carregue os tokens primeiro e depois o componente desejado.

```html
<link rel="stylesheet" href="tokens/tokens.css">
<link rel="stylesheet" href="styles/reset.css">
<link rel="stylesheet" href="components/button/button.css">
```

```html
<button class="btn btn-primary">Falar com a Berry</button>
```

## Convenções

- **Tokens primeiro.** Nenhum componente usa valor cru de cor, medida ou tempo. Tudo referencia `var(--token)`. Para mudar a marca, muda-se o token.
- **Paleta fechada.** Cinco cores de marca (preto, cinza, cinza claro, azul, verde). As únicas exceções são os sinais funcionais de sistema (alerta e erro), restritos a feedback de interface.
- **Fidelidade de vetor.** Logos e ícones foram extraídos dos arquivos oficiais sem regenerar caminho.
- **Fonte única.** O `index.html` carrega o CSS direto das pastas modulares. Para alterar um componente, edita-se o CSS da pasta e o showcase reflete na hora, sem duplicação a manter em sincronia.

## Origem

Este projeto deriva do design system mantido também no Claude Design e da página `berry-design-system.html`. As superfícies devem permanecer em sincronia.
