# Rastreabilidade e Análise de Consistência – US05

### Matriz de Rastreabilidade

| Requisito / User Story | Relacionado a | Descrição / Observações |
|------------------------|---------------|--------------------------|
| US05 - Pagamento com criptomoedas |Módulo de pagamentos, Integração com blockchain, Carteira digital do usuário | O usuário deve poder cadastrar sua carteira digital na plataforma e utilizar criptomoedas para realizar pagamentos. |

---

### Análise de Consistência

- [x] O requisito está descrito de forma clara?
- [x] A plataforma aceita diferentes tipos de criptomoedas?
- [x] Existe um processo de verificação para o cadastro da carteira?
- [ ] A transação em blockchain é vinculada ao pedido e registrada com sucesso?
- [ ] Há tratamento de falhas no momento do pagamento (ex: rede blockchain indisponível)?
- [ ] O sistema valida saldo suficiente antes da confirmação do pedido?

---

### Recomendações

- Utilizar uma API de terceiros confiável para intermediar pagamentos com criptomoedas (ex: Coinbase, BitPay).
- Implementar validação e autenticação ao cadastrar a carteira digital.
- Registrar o hash da transação blockchain na base de dados para rastreabilidade.
- Exibir ao usuário o status da transação em tempo real.
- Criar um histórico de pagamentos com criptomoedas disponível para o usuário.