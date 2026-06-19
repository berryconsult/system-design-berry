# Input / Form Field

Campos de formulário com rótulo, foco em azul, estados de erro e desabilitado.

## Arquivos

- [`input.css`](input.css) — estilos do componente.
- [`input.html`](input.html) — preview isolado (abra no navegador).

## Classes

- `label`
- `input` / `textarea` / `select`
- `.error`

## Variações

- Padrão
- Foco (borda azul + halo 3px)
- Erro (`.error`, vermelho de sistema)
- Desabilitado

## Tokens-chave

`--surface-2`, `--border`, `--azul`, `--cinza-400`, `--r-md`

## Uso

```html
<label for="email">E-mail</label>\n<input id="email" type="email" placeholder="voce@empresa.com.br">
```

> Depende de [`tokens/tokens.css`](../../tokens/tokens.css). Estilos de elemento (foco, reset) vêm de [`styles/`](../../styles/).
