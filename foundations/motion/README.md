# Movimento

Transições curtas e consistentes. O movimento confirma a ação, nunca decora. Um único easing rege todo o sistema.

| Token | Valor | Uso |
|-------|-------|-----|
| `--duration-fast` | 100ms | Microinterações: tags, ícones, badges. |
| `--duration-normal` | 200ms | Padrão: botões, cards, inputs, foco. |
| `--duration-slow` | 300ms | Entradas de seção e estado de carregamento. |
| `--easing-smooth` | cubic-bezier(.4, 0, .2, 1) | Curva padrão. |
| `--easing-bounce` | cubic-bezier(.34, 1.56, .64, 1) | Ênfase pontual. |

O sistema respeita `prefers-reduced-motion`. Quando o usuário pede menos movimento, todas as transições e animações são desligadas.
