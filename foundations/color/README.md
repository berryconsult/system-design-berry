# Cor

A paleta é fechada em cinco cores: três neutros e dois destaques. Nenhuma outra cor de marca é usada.

## As 5 cores

| Cor | Papel | Hex | Token |
|-----|-------|-----|-------|
| Preto | Cor principal | `#000000` | `--preto` |
| Cinza | Cor de apoio | `#7A7A7A` | `--cinza` |
| Cinza Claro | Cor secundária | `#F0F0F0` | `--cinza-claro` |
| Azul | Destaque | `#0D30A4` | `--azul` |
| Verde Berry | Destaque | `#47C97E` | `--verde` |

## Regra de proporção

Os neutros ocupam 90-95% do layout. Azul e verde, juntos ou isolados, ficam em 5-10%. A cor de destaque sinaliza ação e hierarquia; nunca preenche o fundo.

## Escala de neutros

Interfaces densas exigem mais degraus de hierarquia do que um único cinza. A escala `--cinza-900` a `--cinza-050` (`#1A1A1A` a `#F5F5F5`) deriva do mesmo eixo preto-cinza-branco, sem matiz novo. Não são cores adicionais: são tons do neutro, reservados a UI funcional.

## Sinais funcionais de sistema

Fora da paleta de marca, um conjunto mínimo de sinais é usado apenas em feedback de interface, nunca em decoração.

| Sinal | Hex | Token | Observação |
|-------|-----|-------|------------|
| Sucesso | `#47C97E` | `--verde` | O verde da marca já cobre sucesso. |
| Alerta | `#F1C232` | `--warning` | Amarelo de sistema. |
| Erro | `#DC2626` | `--error` | Vermelho de sistema. |

## Tema claro e escuro

O sistema nasce escuro. O tema claro inverte apenas o eixo neutro: o fundo passa a branco, o texto assume o quase-preto e as superfícies viram o mesmo cinza com baixa opacidade sobre o branco. A paleta de marca permanece fechada.

O acento acompanha o contraste. Em fundo escuro o verde lidera os acentos pequenos, porque o azul perde leitura em texto miúdo. Em fundo claro a relação se inverte: o azul assume acentos e títulos, o verde fica em preenchimentos e no estado de sucesso. Para escrita em azul sobre escuro, use `--azul-text` (`#3373F5`), que recupera contraste.
