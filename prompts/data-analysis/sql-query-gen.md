# 📝 Geração de Query SQL

## Descrição
Este prompt é usado para gerar queries SQL complexas (SELECT, INSERT, UPDATE, etc.) a partir de uma descrição em linguagem natural. É crucial incluir o esquema da tabela (nomes das colunas e tipos de dados) para resultados precisos.

## Estrutura do Prompt
**Exemplo:**
- Gere uma query SQL que retorne o nome do cliente e a soma total de seus pedidos. Use as tabelas 'clientes' (colunas: id_cliente, nome) e 'pedidos' (colunas: id_pedido, id_cliente, valor_total).

## Resultado Esperado
```sql
SELECT c.nome, SUM(p.valor_total) AS total_gasto
FROM clientes c
JOIN pedidos p ON c.id_cliente = p.id_cliente
GROUP BY c.nome;