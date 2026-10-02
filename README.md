# workshop_dados_pratica
# Case Café Tambaú ☕

O **Café Tambaú** é uma cafeteria na orla de João Pessoa. Ela atende no balcão e por delivery (iFood) e tem um programa de fidelidade.

Em agosto e setembro de 2026, o dono percebeu que o caixa estava mais vazio do que no começo do ano. Ele te contratou para responder:

> **Por que as vendas caíram e o que eu devo fazer?**

Os dados cobrem de **janeiro a setembro de 2026**.

## Pastas

- `dados_brutos/`: os dados como saíram do sistema da cafeteria, com problemas de qualidade. É por aqui que a Prática 1 (Engenharia de Dados) começa.
- `dados_tratados/`: os mesmos dados já limpos. Use se quiser pular direto para a Análise, a Ciência ou a IA.

## Dicionário de dados

### vendas.csv (uma linha por item vendido)
| Coluna | Descrição |
|---|---|
| id_venda | Código do pedido. Um pedido pode ter vários itens |
| data_hora | Data e hora da venda |
| id_cliente | Código do cliente. Vazio quando o cliente não se identificou |
| id_produto | Código do produto (ver produtos.csv) |
| quantidade | Quantidade do item |
| preco_unitario | Preço cobrado por unidade, em reais |
| canal | Balcão ou iFood |
| forma_pagamento | Pix, cartão, dinheiro ou iFood (online) |
| tempo_entrega_min | Tempo de entrega em minutos (só pedidos do iFood) |

### produtos.csv
| Coluna | Descrição |
|---|---|
| id_produto | Código do produto |
| nome_produto | Nome no cardápio |
| categoria | Bebida quente, bebida fria, salgado ou doce |
| custo_unitario | Quanto custa para a cafeteria produzir uma unidade |
| preco_atual | Preço de venda atual |

### historico_precos.csv
Preço de cada produto e o período em que ele valeu.

### clientes.csv
| Coluna | Descrição |
|---|---|
| id_cliente | Código do cliente |
| nome | Nome do cliente (fictício) |
| bairro | Bairro de João Pessoa onde mora |
| data_cadastro | Data em que entrou no cadastro |
| programa_fidelidade | Se participa do programa de fidelidade |
| idade | Idade em anos |
| email | E-mail (fictício) |

### avaliacoes.csv
| Coluna | Descrição |
|---|---|
| id_avaliacao | Código da avaliação |
| data_avaliacao | Data e hora da avaliação |
| id_venda | Pedido avaliado |
| id_cliente | Cliente que avaliou (pode estar vazio) |
| canal | Canal do pedido |
| nota | Nota de 1 a 5 |
| comentario | Texto escrito pelo cliente |

Todos os dados são fictícios e foram criados para fins didáticos pelo Nerd Data Lab.
