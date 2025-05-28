### História de Usuário 1

**Como** administrador da plataforma  
**Quero** que avaliações sejam armazenados em blockchain   
**Para** garantir a integridade dos dados.   

---

#### Critérios de Aceitação

- [ ]  Todas as avaliações de produto devem ser registradas na blockchain automaticamente.
- [ ]  O registro na blockchain deve acontecer sem impactar negativamente o tempo de resposta da plataforma (ex: registro assíncrono ou otimizado).
- [ ]  Caso o registro de uma avaliação na blockchain falhe, o sistema deve armazená-la como pendente e realizar novas tentativas automáticas de registro a cada 3 horas, por no máximo 5 vezes. Caso a transação continue falhando, o sistema deve notificá-la como erro crítico no painel administrativo.

#### Notas Técnicas

