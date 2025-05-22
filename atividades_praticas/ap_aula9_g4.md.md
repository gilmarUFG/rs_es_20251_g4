# Matriz de Rastreabilidade de Requisitos

## Introdução
A Matriz de Rastreabilidade de Requisitos (MRR) é uma ferramenta que permite mapear a relação entre os requisitos do projeto e suas implementações, testes e outras fases do ciclo de vida do desenvolvimento.

## Estrutura

| ID      | Descrição                                                                                                         | Fonte                        | Caso de Teste | Status        | Comentários                                                        |
|---------|------------------------------------------------------------------------------------------------------------------|------------------------------|---------------|---------------|--------------------------------------------------------------------|
| REQ-001 | O sistema deve armazenar avaliações e comentários na blockchain.                                                               | Mauro Sérgio (Cliente), HU-01 | CT-001        | Em progresso  | Validar armazenamento e exibição correta das avaliações.           |
| REQ-002 | O sistema deve registrar as transações para garantir a rastreabilidade, autenticidade e segurança.               | Giovanna Lysa (Cliente), [HU-02](/trabalho_final/historias_usuarios/hu2)      | CT-002        | Concluído     | Confirmar registro seguro e rastreável das transações.             |
| REQ-003 | O sistema deve oferecer um mecanismo de autentificação para vendedores.                                           | José Alves (Cliente)         | CT-003        | Em progresso  | Revisar autenticação e segurança das credenciais dos vendedores.   |
| REQ-004 | O sistema deve permitir que os usuários acompanhem o status da entrega de seus pedidos em tempo real, com atualizações armazenadas diretamente na blockchain. | Sophia Fernandes (Cliente), [HU-04](/trabalho_final/historias_usuarios/hu4)   | CT-004        | Não iniciado  | Implementar integração com blockchain para rastreamento de pedidos.|
| REQ-005 | O sistema deve permitir que o usuário cadastre sua carteira digital para utilizar criptomoedas na realização de pagamentos. | Guilherme Gonçalves (Cliente) | CT-005        | Em progresso  | Garantir validação e segurança no cadastro da carteira digital.    |
| REQ-006 | O sistema não deve permitir a venda de um produto caso o vendedor não o tenha mais em estoque.                   | Leonardo Moreira (Cliente), [HU-06](/trabalho_final/historias_usuarios/hu6)   | CT-006        | Em progresso  | Validar bloqueio de vendas para produtos sem estoque.              |
| REQ-007 | O sistema deve registrar as atualizações de status de um pedido na blockchain.                                   | José Carlos (Cliente)        | CT-007        | Em progresso  | Verificar registro correto das atualizações na blockchain.         |
| REQ-008 | O sistema deve mostrar as especificações dos produtos aos compradores.                                           | Gabriel Borges (Cliente), [HU-08](/trabalho_final/historias_usuarios/hu8)     | CT-008        | Em progresso  | Conferir exibição detalhada das especificações dos produtos.       |
| REQ-009 | O sistema deve atualizar automaticamente o estoque dos produtos conforme as compras são realizadas.              | Aline Lima (Cliente), [HU-09](/trabalho_final/historias_usuarios/hu9)         | CT-009        | Em progresso  | Testar atualização automática do estoque após cada compra.         |
| REQ-010 | O sistema deve permitir que o usuário salve suas informações de cartões bancários de forma segura para as próximas compras. | Aline Ayumi (Cliente)        | CT-010        | Em progresso  | Garantir armazenamento seguro dos dados dos cartões bancários.     |

## Legenda
- **ID**: Identificador único para cada requisito.
- **Descrição**: Detalhamento do que o requisito envolve.
- **Fonte**: Origem do requisito, como documentos ou reuniões de stakeholders.
- **Caso de Teste**: ID do caso de teste relacionado para validação do requisito.
- **Status**: Estado atual do requisito (Em progresso, Concluído, Não iniciado).
- **Comentários**: Observações ou pontos relevantes sobre o requisito ou sua implementação.
