# barcelona

viagem barcelona

Mapa online: https://jvbrilhant.github.io/barcelona/

Mapa de atrações de Barcelona com Leaflet e OpenStreetMap.

- `index.html`: a página (não precisa editar).
- `places.json`: os lugares. Edite aqui para adicionar, remover ou corrigir pins.

## Campos de cada lugar em `places.json`

| Campo | O que é |
|---|---|
| `nome` | Nome exibido no pin e no popup |
| `lat`, `lon` | Coordenadas |
| `tipo` | `paid` (paga, vermelho), `free` (grátis, verde) ou `food` (comer e beber, cinza) |
| `texto` | Descrição e preços, mostrados no popup |
| `aproximado` | `true` desenha o pin com borda tracejada (posição aproximada) |
| `precoMin` | Só para `paid`: preço mínimo em euros (número) ou `null` se não informado |
| `linkIngresso` | Só para `paid`: link para comprar o ingresso |

Depois de editar, confira se o JSON continua válido (vírgulas e aspas). Se o arquivo tiver erro, a página mostra um aviso no topo.

## Rodar no computador

O navegador não deixa a página ler `places.json` quando o `index.html` é aberto direto do disco. Rode um servidor local na pasta:

```bash
python3 -m http.server 8000
```

e abra http://localhost:8000.
