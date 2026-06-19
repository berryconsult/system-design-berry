# Tipografia

Duas famílias, papéis fixos. É o par definido no manual.

| Família | Papel | Peso principal | Token |
|---------|-------|----------------|-------|
| IBM Plex Sans | Títulos e subtítulos | Medium (500) | `--font-display` |
| Inter | Corpo de texto | Regular (400) | `--font-body` |
| IBM Plex Mono | Código, rótulos técnicos, kickers | Regular/Medium | `--font-mono` |

## Escala

| Estilo | Família · peso · tamanho | Token |
|--------|--------------------------|-------|
| Display XL | IBM Plex Sans · 600 · 72px · tracking -2% | `--fs-display-xl` |
| Display LG | IBM Plex Sans · 500 · 52px | `--fs-display-lg` |
| Heading 1 | IBM Plex Sans · 500 · 40px | `--fs-h1` |
| Heading 2 | IBM Plex Sans · 500 · 28px | `--fs-h2` |
| Heading 3 | IBM Plex Sans · 500 · 22px | `--fs-h3` |
| Lead | Inter · 400 · 18px | `--fs-lg` |
| Body | Inter · 400 · 16px | `--fs-base` |
| Eyebrow / Label | Inter · 600 · 12px · uppercase · tracking +14% | `--fs-xs` |

Não inverta os papéis: IBM Plex Sans Medium em títulos, Inter Regular no corpo. Os tamanhos display usam `clamp()` para escalar com a viewport.
