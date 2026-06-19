# Superfícies e brilho

A profundidade vem do tom da superfície e de uma hairline de 1px, não de sombras pesadas.

As superfícies são o Cinza com baixa opacidade sobre o Preto. Três níveis:

| Token | Cinza sobre preto | Uso |
|-------|-------------------|-----|
| `--surface-1` | ~4,5% | Fundo mais sutil. |
| `--surface-2` | ~8% | Card padrão. |
| `--surface-3` | ~13% | Card destacado ou hover. |

As bordas seguem a mesma lógica: `--border` (cinza a 26%) e `--border-strong` (40%).

A profundidade nasce de três camadas: o tom da superfície, a hairline de 1px e um realce radial neutro (branco com baixíssima opacidade) que parte do centro, com leve brilho na aresta superior. O brilho azul de marca (`--glow`) fica reservado aos cards de destaque, não às superfícies neutras.
