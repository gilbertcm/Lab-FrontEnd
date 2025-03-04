# CSS Grid

O CSS Grid é um modelo de layout poderoso que permite criar designs complexos com facilidade, organizando elementos em linhas e colunas.

## Propriedades do CSS Grid

### 1. Definição do Contêiner Grid

#### `display`
- `grid` → Define o elemento como um contêiner Grid.
- `inline-grid` → Define o contêiner Grid como um elemento inline.

#### `grid-template-columns`
Define o número e o tamanho das colunas:
- `grid-template-columns: 100px 200px;` → Cria duas colunas com larguras fixas.
- `grid-template-columns: 1fr 2fr;` → Usa frações do espaço disponível.

#### `grid-template-rows`
Define o número e o tamanho das linhas:
- `grid-template-rows: 100px 200px;` → Cria duas linhas com alturas fixas.
- `grid-template-rows: auto 1fr;` → A primeira linha ajusta-se ao conteúdo e a segunda ocupa o espaço restante.

#### `grid-template-areas`
Define áreas nomeadas para organização do layout:
```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar content"
    "footer footer";
}
```

#### `gap`
Define o espaçamento entre as células do grid:
- `row-gap: 10px;` → Define espaçamento entre as linhas.
- `column-gap: 20px;` → Define espaçamento entre as colunas.
- `gap: 10px 20px;` → Define espaçamento entre linhas e colunas.

#### `justify-items`
Define o alinhamento dos itens dentro das células:
- `start` → Alinha os itens no início da célula.
- `center` → Centraliza os itens.
- `end` → Alinha os itens no final da célula.
- `stretch` (padrão) → Os itens expandem para ocupar toda a célula.

#### `align-items`
Define o alinhamento vertical dos itens:
- `start`, `center`, `end`, `stretch` (padrão).

#### `place-items`
Atalho para `align-items` e `justify-items`:
- `place-items: center;` → Centraliza os itens horizontal e verticalmente.

#### `justify-content`
Define o alinhamento do grid dentro do contêiner:
- `start`, `center`, `end`, `space-between`, `space-around`, `space-evenly`.

#### `align-content`
Define o alinhamento das linhas do grid dentro do contêiner:
- `start`, `center`, `end`, `space-between`, `space-around`, `stretch` (padrão).

### 2. Propriedades dos Itens Grid

#### `grid-column`
Define a posição do item nas colunas:
- `grid-column: 1 / 3;` → O item ocupa da coluna 1 até a 3.

#### `grid-row`
Define a posição do item nas linhas:
- `grid-row: 2 / 4;` → O item ocupa da linha 2 até a 4.

#### `grid-area`
Define a posição do item usando `grid-template-areas`:
```css
.item {
  grid-area: header;
}
```