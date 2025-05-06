### História de Usuário 2

**Como** vendedor do ecommerce
**Quero** que os meus produtos cujo estoque tenha acabado saiam automaticamente de comercialização
**Para**  evitar realizar vendas de produtos que não possuo em estoque.

---

#### Critérios de Aceitação

- [ ] Uma vez que o estoque chegue a zero, o status do produto começa a aparecer como indisponível.
- [ ] Um e-mail deve ser enviado ao vendedor, notificando o esgotamento do produto.
- [ ] Uma vez fora de estoque, o produto deverá ser removido dos carrinhos em que anteriormente foi colocado.
- [ ] A remoção do produto deve ser transparente para o cliente(Uma mensagem fixa de “Este item não está mais disponível e foi removido do seu carrinho”).

#### Notas Técnicas

- É necessário garantir que o sistema de carrinho seja capaz de identificar e remover automaticamente produtos esgotados.
- Certificar-se de que a lógica de indisponibilidade esteja sincronizada com possíveis caches usados no frontend ou sistemas de busca (como Elasticsearch).
  