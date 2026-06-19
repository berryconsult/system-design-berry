# Icon Badge

Conjunto oficial de ícones em badge: glifo branco em relevo sobre tile escuro, geometria Lucide.

## Arquivos

- [`icon-badge.css`](icon-badge.css) — estilos do componente.
- [`icon-badge.html`](icon-badge.html) — preview isolado (abra no navegador).

## Classes

- `.icon-grid`
- `.icon-cell`
- `.ico-badge`

## Variações

- Badge (relevo)
- Monocromático (em interface densa, herda o acento)

## Tokens-chave

`#ico-grad (gradiente)`, `--fs-xs`, `--txt-2`

## Uso

```html
<span class="ico-badge"><svg viewBox="0 0 150 150"><path d="..."/></svg></span>
```

> Depende de [`tokens/tokens.css`](../../tokens/tokens.css). Estilos de elemento (foco, reset) vêm de [`styles/`](../../styles/).
