# Rastreabilidade e Análise de Consistência – US04

### Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a | Descrição / Observações |
|------------------------|---------------|--------------------------|
| US04 - Acompanhamento de entrega em tempo real | Sistema de rastreamento de pedidos, Integração com blockchain, Experiência do usuário | A plataforma deve permitir que os usuários acompanhem o status da entrega de seus pedidos em tempo real, com atualizações armazenadas diretamente na blockchain. |

---

### Análise de Consistência

- [x] O requisito foi descrito de forma clara e objetiva?
- [x] As atualizações de status são persistidas de forma imutável?
- [x] A visualização do status é em tempo real para o usuário?
- [ ] Existe fallback caso a blockchain esteja temporariamente indisponível?
- [ ] Há validação das fontes de atualização de status (logística integrada)?
- [ ] Os dados exibidos ao usuário são consistentes com os registros em blockchain?



### Recomendações

- Utilizar uma blockchain permissionada para otimizar performance nas atualizações frequentes.
- Implementar mecanismos de cache/local storage para minimizar impacto em caso de falha na consulta.
- Integrar com APIs de logística para rastrear eventos como "pedido enviado", "em trânsito", "entregue".
- Garantir que cada atualização gere um hash único e inviolável armazenado na blockchain.
- Permitir ao usuário visualizar o histórico completo de movimentações do pedido.