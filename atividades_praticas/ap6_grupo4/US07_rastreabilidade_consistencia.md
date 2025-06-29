# Rastreabilidade e Análise de Consistência – US06

### Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a | Descrição / Observações |
|------------------------|---------------|--------------------------|
| US07 - Visualização do histórico imutável de transações | Histórico de pedidos, Blockchain, Transparência para comprador | O sistema deve permitir que o comprador visualize o histórico imutável de transações de um pedido (ex: pagamento confirmado, envio, entrega) registrado na blockchain. |

---

### Análise de Consistência

- [x] O requisito está descrito de forma clara e objetiva?
- [x] O histórico é armazenado de forma imutável na blockchain?
- [x] A interface do usuário apresenta o histórico completo e atualizado?
- [ ] Existe autenticação para garantir que somente o comprador acesse seu histórico?
- [ ] Há mecanismo para lidar com falhas na recuperação dos dados da blockchain?
- [ ] Os eventos do histórico são atualizados em tempo real?

---

### Recomendações

- Garantir que todas as etapas da transação sejam registradas na blockchain com timestamps.
- Disponibilizar uma interface amigável para o comprador consultar o histórico.
- Implementar autenticação robusta para garantir a privacidade dos dados.
- Utilizar caching para otimizar consultas frequentes ao histórico.
- Fornecer notificações ao comprador quando houver atualização no status do pedido.
