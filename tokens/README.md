# Tokens

A fonte única de verdade do sistema. Toda cor, medida, fonte e tempo vive aqui; componentes e foundations apenas referenciam.

## Arquivos

| Arquivo | Papel |
|---------|-------|
| [`tokens.json`](tokens.json) | Fonte estruturada em formato [W3C Design Tokens (DTCG)](https://www.designtokens.org/). Legível por máquina, agnóstica de plataforma. |
| [`tokens.css`](tokens.css) | Espelho em CSS custom properties (`:root`) mais o tema claro (`html.light`). É o que os componentes e previews consomem. |

## Camadas

Os tokens são organizados em camadas, da mais bruta à mais semântica:

1. **Primitivas** — os valores crus: as 5 cores da marca, a escala de neutros, os sinais funcionais.
2. **Semânticas** — apelidos de papel: `bg`, `text`, `accent`, que mudam com o tema.
3. **Tema** — o bloco `html.light` inverte apenas o eixo neutro e troca o acento de verde para azul. A paleta de marca permanece fechada.

## Como consumir

Em qualquer página ou componente, carregue o CSS antes de tudo:

```html
<link rel="stylesheet" href="tokens/tokens.css">
```

Depois use as variáveis:

```css
.botao { background: var(--azul); border-radius: var(--r-sm); transition: all var(--duration-normal) var(--easing-smooth); }
```

## Build opcional

`tokens.json` está pronto para o [Style Dictionary](https://amzn.github.io/style-dictionary/) ou ferramenta equivalente, caso se queira gerar saídas para iOS, Android, Tailwind ou Figma a partir da mesma fonte. O `tokens.css` deste repositório é o equivalente já compilado para a web.
