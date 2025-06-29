### História de Usuário 9

**Como** cliente do sistema  
**Quero** que o estoque dos produtos seja atualizado automaticamente após cada compra  
**Para** evitar a venda de produtos fora de estoque e garantir informações atualizadas.

---

#### Critérios de Aceitação

- [ ] O estoque do produto é reduzido corretamente após a finalização de uma compra  
- [ ] O sistema não permite compras de produtos com estoque insuficiente  
- [ ] A atualização do estoque deve ser refletida imediatamente na interface de administração e no catálogo do cliente

#### Notas Técnicas

- A lógica de atualização deve ser executada após a confirmação de pagamento (compra finalizada com sucesso)  
- O sistema deve lidar com concorrência para evitar problemas de estoque negativo (ex: lock em banco de dados ou transações)  
- Integrar com a camada de compras/pedidos e garantir rollback em caso de falha na transação  
- Dependência: módulo de pedidos finalizados e módulo de estoque devem estar implementados  
- Recomendado: testes automatizados para garantir a integridade da lógica de estoque
