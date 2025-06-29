# Rastreabilidade e Análise de Consistência – US06

### Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a | Descrição / Observações |
|------------------------|---------------|--------------------------|
| US06 - Controle de estoque para venda | Sistema de estoque, Processo de venda, Segurança de transações | O sistema não deve permitir a venda de um produto caso o vendedor não o tenha mais em estoque. |

---

### Análise de Consistência

- [x] O requisito está descrito de forma clara?
- [x] O sistema verifica o estoque em tempo real antes da confirmação da venda?
- [ ] Existe atualização automática do estoque após a venda?
- [ ] Há mecanismo para evitar vendas simultâneas que causem estoque negativo?
- [ ] O sistema bloqueia a venda quando o estoque é insuficiente?
- [ ] O processo de atualização do estoque é registrado para auditoria?

---

### Recomendações

- Implementar checagem de estoque no momento do checkout para garantir disponibilidade.
- Atualizar o estoque imediatamente após a conclusão da venda para evitar inconsistências.
- Utilizar bloqueios ou transações atômicas para evitar vendas simultâneas que excedam o estoque.
- Registrar cada alteração de estoque com timestamp para rastreabilidade e auditoria.
- Notificar o vendedor e o comprador quando um produto estiver indisponível para venda.