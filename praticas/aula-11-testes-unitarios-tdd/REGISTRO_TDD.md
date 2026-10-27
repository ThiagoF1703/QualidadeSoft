# Registro do ciclo de TDD

## Comportamento escolhido

Calcular a taxa de entrega de acordo com a distância percorrida e o valor total do pedido.

## Red

**Teste criado:** `test_taxa_entrega_ate_3_km`

**Motivo da falha:** A função `calcular_taxa_entrega` ainda não estava implementada, portanto não era possível calcular a taxa de entrega esperada de R$ 5,00 para uma distância de 2 km.

## Green

**Implementação realizada:** Foi criada a função `calcular_taxa_entrega`, que cobra R$ 5,00 para distâncias de até 3 km, acrescenta R$ 2,00 por quilômetro excedente e oferece entrega gratuita para pedidos a partir de R$ 100,00.

Também foi adicionada a validação para impedir distâncias negativas.

## Refactor

**Melhoria realizada:** A implementação foi organizada em condições simples para facilitar a leitura e a manutenção do código. Não foi necessária uma refatoração adicional.

**Resultado final:** Foram criados testes para os três cenários obrigatórios: entrega até 3 km, entrega acima de 3 km e entrega gratuita para pedidos a partir de R$ 100,00. Também foi incluído um teste opcional para distância negativa. A aprovação de todos os testes depende da execução da suíte de testes.