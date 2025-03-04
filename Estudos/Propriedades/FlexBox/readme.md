# Flexbox CSS

O Flexbox (Flexible Box) é um modelo de layout no CSS que permite criar interfaces responsivas e organizadas de forma eficiente. Ele facilita a distribuição e o alinhamento dos elementos dentro de um contêiner flexível.

## Propriedades do Flexbox

### 1. Propriedades do Contêiner Flexível

#### `display`
- `display: flex;` → Define o elemento como um contêiner flexível.
- `display: inline-flex;` → Define o contêiner como um elemento inline flexível.

#### `flex-direction`
Define a direção dos itens dentro do contêiner:
- `row` (padrão) → Direção da esquerda para a direita.
- `row-reverse` → Direção da direita para a esquerda.
- `column` → Direção de cima para baixo.
- `column-reverse` → Direção de baixo para cima.

#### `flex-wrap`
Define se os itens devem quebrar para a próxima linha:
- `nowrap` (padrão) → Todos os itens ficam em uma única linha.
- `wrap` → Os itens quebram para uma nova linha conforme necessário.
- `wrap-reverse` → Igual ao `wrap`, mas na direção inversa.

#### `justify-content`
Alinha os itens ao longo do eixo principal:
- `flex-start` (padrão) → Alinha os itens no início do contêiner.
- `flex-end` → Alinha os itens no final do contêiner.
- `center` → Centraliza os itens.
- `space-between` → Distribui os itens com espaço igual entre eles.
- `space-around` → Distribui os itens com espaço ao redor de cada um.
- `space-evenly` → Distribui os itens com espaços uniformes.

#### `align-items`
Alinha os itens ao longo do eixo transversal:
- `stretch` (padrão) → Itens esticam para preencher o contêiner.
- `flex-start` → Alinha os itens no início do eixo transversal.
- `flex-end` → Alinha os itens no final do eixo transversal.
- `center` → Centraliza os itens verticalmente.
- `baseline` → Alinha os itens pela linha base do texto.

#### `align-content`
Controla o espaçamento entre linhas quando há várias linhas de itens flexíveis:
- `flex-start` → Alinha as linhas no topo do contêiner.
- `flex-end` → Alinha as linhas na parte inferior.
- `center` → Centraliza as linhas.
- `space-between` → Distribui as linhas com espaço igual entre elas.
- `space-around` → Distribui as linhas com espaço ao redor de cada uma.
- `stretch` (padrão) → As linhas esticam para preencher o espaço disponível.

### 2. Propriedades dos Itens Flexíveis

#### `flex-grow`
Define a capacidade do item de crescer para ocupar o espaço disponível:
- `0` (padrão) → O item não cresce.
- `1` → O item pode crescer para ocupar o espaço disponível.

#### `flex-shrink`
Define a capacidade do item de encolher caso o espaço seja insuficiente:
- `1` (padrão) → O item pode encolher se necessário.
- `0` → O item não encolhe.

#### `flex-basis`
Define o tamanho inicial do item antes da aplicação de `grow` ou `shrink`:
- Valores podem ser `auto`, um tamanho específico (`px`, `%`, etc.).

#### `align-self`
Permite sobrescrever o `align-items` para um item específico:
- `auto` (padrão) → Usa o valor do `align-items` do contêiner.
- `flex-start`, `flex-end`, `center`, `baseline`, `stretch` → Comportamento semelhante ao `align-items`.
