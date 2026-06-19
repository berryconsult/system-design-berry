# Theme Toggle

Botão fixo que alterna entre tema escuro e claro e memoriza a escolha em localStorage.

## Arquivos

- [`theme-toggle.css`](theme-toggle.css) — estilos do componente.
- [`theme-toggle.html`](theme-toggle.html) — preview isolado (abra no navegador).

## Classes

- `.theme-toggle`
- `.ic-moon` / `.ic-sun`
- `.lbl`

## Variações

- Escuro (padrão)
- Claro (classe `.light` no `<html>`)

## Tokens-chave

`--surface-2`, `--border`, `--r-pill`, `--duration-normal`

## Uso

```html
<button class="theme-toggle" type="button" aria-pressed="false">\n  <svg class="ic-moon" ...></svg><span class="lbl"></span>\n</button>
```

> Depende de [`tokens/tokens.css`](../../tokens/tokens.css). Estilos de elemento (foco, reset) vêm de [`styles/`](../../styles/).
