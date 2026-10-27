# Consulta de CFOP

Página para consultar qual CFOP usar na entrada de uma nota recebida e quais CFOPs usar nas saídas seguintes (retorno, devolução, venda), para operações de remessa, consignação, industrialização por encomenda, conserto, demonstração, comodato, armazém geral, venda à ordem, entrega futura, compras, transferências e exportação indireta.

## Como usar

Digite o CFOP que está na nota recebida (ex.: `6.917`) ou uma palavra-chave (ex.: `conserto`). Também aceita CFOP de entrada (`1.xxx` / `2.xxx`).

## Publicar no GitHub Pages

1. Envie `index.html` para a raiz do repositório (branch `main`).
2. Em **Settings → Pages**, em *Source*, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e salve.
3. Em alguns minutos o site fica disponível em `https://SEU-USUARIO.github.io/NOME-DO-REPOSITORIO/`.

## Editar as operações

Todas as operações ficam na constante `OPS`, no `<script>` do `index.html`. Cada item tem:

- `r`: finais dos CFOPs da nota recebida (ex.: `"917"`)
- `e`: CFOPs de entrada (`c` = final, `d` = descrição, `w` = quando usar)
- `s`: CFOPs das saídas seguintes (`dest`: `origem`, `cliente`, `exterior` ou `fixo`)
- `n`: observações

## Aviso

Referência baseada na tabela de CFOP (Convênio s/nº de 1970, Ajuste SINIEF 07/01) e no Ajuste SINIEF 02/93. Alguns estados têm regras próprias. Confirme com o contador responsável em caso de dúvida.
