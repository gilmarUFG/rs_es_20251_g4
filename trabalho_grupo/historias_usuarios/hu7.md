## História de Usuário 7

**Como** comprador do e-commerce  
**Quero** visualizar o histórico imutável de transações de um pedido registrado na blockchain  
**Para** ter transparência e confiança no acompanhamento do status da minha compra

### Critérios de Aceitação

- O comprador deve poder acessar uma linha do tempo do pedido com eventos como: pagamento confirmado, pedido enviado e pedido entregue.  
- Cada evento da linha do tempo deve estar vinculado a um registro imutável na blockchain.  
- As informações devem incluir data/hora, tipo de evento e o hash da transação correspondente.  
- O sistema deve exibir mensagens claras quando a transação ainda não tiver sido registrada na blockchain ou estiver em confirmação.

### Notas Técnicas

- Integrar com API de blockchain para registrar e consultar transações.
- Utilizar smart contracts ou serviços de terceiros para registrar eventos relevantes na blockchain.
- Armazenar localmente os hashes das transações vinculados aos pedidos no banco de dados.
- A estratégia de blockchain adotada para registro de eventos será definida conforme requisitos de custo, escalabilidade e privacidade. 
