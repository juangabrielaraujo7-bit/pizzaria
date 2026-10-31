# Cardápio digital da pizzaria

Site estático responsivo com 46 opções de produtos: pizzas, combos, bebidas, hambúrgueres, porções, massas e sobremesas.

## Executar

Abra `dist/index.html` ou sirva a pasta `dist` com um servidor HTTP estático. Não há dependências nem compilação. Na Vercel, importe a raiz do repositório: `vercel.json` configura a saída `dist`.

## Recursos

- Busca e navegação por categorias.
- Tamanhos, sabores, bordas, adicionais e observações conforme o produto.
- Sacola com alteração de quantidades, remoção e total.
- Checkout com contato, endereço, entrega ou retirada e revisão.
- Pix, cartão e pagamento no recebimento em demonstração.
- Cupom `BEMVINDO10`: 10% sobre os produtos, sem desconto no frete.
- Frete demonstrativo fixo de R$ 8,00 e retirada gratuita.
- Troco com validação do valor.
- Confirmação, histórico local dos últimos 20 pedidos e acompanhamento manual simulado.

## Demonstração

Não processa pagamentos, não gera Pix real e não envia pedidos à loja. Não solicita dados de cartão. Os dados de contato e endereço ficam somente na memória da sessão; o histórico local não inclui contato, endereço ou observações. A sacola fica salva no navegador até ser concluída ou removida.

Antes de receber pedidos reais, configurar identidade da loja, endereço, horários, cobertura e taxas, catálogo, servidor de pedidos e integração de pagamentos com verificação no servidor. As imagens de pizzas e bebidas usam endereços externos da referência; novos produtos usam ilustrações com emoji.

## Arquivos

- `dist/index.html`: estrutura.
- `dist/style.css` e `dist/checkout.css`: aparência e layout responsivo.
- `dist/app.js`: cardápio inicial e sacola.
- `dist/checkout.js`: catálogo ampliado, checkout e pedidos demonstrativos.
