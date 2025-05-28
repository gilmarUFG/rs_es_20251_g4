### História de Usuário 3

**Como** administrador da plataforma  
**Quero** que o sistema ofereça um mecanismo de autentificação para vendedores  
**Para** garantir que apenas vendedores legítimos possam anunciar produtos e reduzir o risco de fraude.

---

#### Critérios de Aceitação

- [ ] O sistema deve exigir autentificação dos vendedores antes de permitir o cadastro ou anúncio de produtos.
- [ ] O processo de autentificação deve validar documentos e informações cadastrais do vendedor.
- [ ] Caso a autentificação falhe ou haja suspeita de fraude, o cadastro deve ser bloqueado e o administrador notificado.
- [ ] O vendedor deve ser informado sobre o status da autentificação (aprovado, pendente, rejeitado).

#### Notas Técnicas

- Implementar integração com serviço de validação de documentos (ex: consulta CNPJ/CPF).
- Utilizar autenticação em dois fatores (2FA) para acesso ao painel do vendedor.
- Registrar logs de todas as tentativas de autentificação e alterações cadastrais.
- Garantir armazenamento seguro dos dados sensíveis dos vendedores.