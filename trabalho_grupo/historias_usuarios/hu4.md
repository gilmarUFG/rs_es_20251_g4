### História de Usuário 4

**Como** cliente do e-commerce  
**Quero** visualizar o histórico de status de entrega do meu pedido em tempo real  
**Para** acompanhar o processo logístico e saber onde está minha encomenda.

---

> Nota: Esta história foca exclusivamente nos eventos de entrega (ex: pedido enviado, em trânsito, entregue). Para visualizar todos os eventos do pedido (incluindo pagamento, reembolso, etc.), consulte HU7.

#### Critérios de Aceitação

- [ ] O usuário deve conseguir visualizar o histórico completo de atualizações de entrega do pedido, em ordem cronológica, com data/hora, status e localização (cidade/estado) de cada evento.
- [ ] O sistema deve registrar cada atualização de entrega na blockchain, garantindo que o histórico seja imutável (não pode ser alterado, apenas adicionado um novo evento com timestamp).
- [ ] O status atual da entrega deve ser destacado na interface.

#### Notas Técnicas

- Necessária integração com a API da transportadora para obter atualizações de entrega.
- As atualizações de entrega devem ser registradas na blockchain conforme estratégia definida para o projeto.
