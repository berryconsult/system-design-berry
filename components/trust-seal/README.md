# Trust Seal

Selos de parceiros reconhecíveis (Google, ReclameAQUI, Meta). Use o selo oficial, não só texto.

## Arquivos

- [`trust-seal.css`](trust-seal.css) — estilos do componente.
- [`trust-seal.html`](trust-seal.html) — preview isolado (abra no navegador).

## Classes

- `.trust-row`
- `.seal`
- `.mark`
- `.gword`
- `.t1` / `.t2`

## Variações

- Padrão (fundo claro)

## Tokens-chave

`--r-md`, `--font-display`

## Uso

```html
<div class="seal"><span class="mark">...</span><span class="txt"><span class="t1">Meta</span><span class="t2">Business Partner</span></span></div>
```

> Depende de [`tokens/tokens.css`](../../tokens/tokens.css). Estilos de elemento (foco, reset) vêm de [`styles/`](../../styles/).
