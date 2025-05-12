### História de Usuário 2

**Como** administrador da plataforma
**Quero** que todas as transações sejam registradas automaticamente 
**Para** garantir a rastreabilidade, autenticidade e segurança das operações.
---

#### Critérios de Aceitação

- [ ] Todas as transações relevantes devem ser registradas na blockchain automaticamente.
- [ ] O administrador deve ter acesso a um painel ou mecanismo de consulta que permita verificar o status de cada transação registrada (confirmada, pendente, falha).
- [ ] Caso uma transação falhe ao ser registrada na blockchain, o sistema deve armazená-la como pendente e realizar novas tentativas automáticas de registro a cada 3 horas, por no máximo 5 vezes. Caso a transação continue falhando, o sistema deve notificá-la como erro crítico no painel administrativo.

#### Notas Técnicas

- As transações na blockchain devem possuir assinaturas digitais com chaves privadas.
- Necessário implementar uma fila de tarefas pendentes (ex: RabbitMQ, Redis, ou uma tabela no banco de dados).
