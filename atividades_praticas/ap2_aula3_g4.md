# Requisito Funcional: RF004 -  O software deve possibilitar o registro de livros com título, autor, editora, categoria.

## 1. Descrição
O sistema deve permitir o cadastro de livros, garantindo que todas as informações essenciais sejam registradas corretamente. Esse requisito assegura que os usuários possam adicionar novos livros ao catálogo de forma organizada e padronizada.

## 1. Identificação das Fontes
- Bibliotecário, administrador do sistema, funcionário responsável pelo cadastro de livros

## 2. Detalhamento

- **Ator(es):** Usuário com permissão de cadastro (ex.: administrador, bibliotecário).  

- **Entrada:** Dados obrigatórios para o registro do livro:  
  - **Título:** Nome do livro, preenchimento obrigatório.  
  - **Autor:** Nome(s) do(s) autor(es) do livro, preenchimento obrigatório.  
  - **Editora:** Nome da editora responsável pela publicação, preenchimento obrigatório.  
  - **Categoria:** Classificação do livro (ex.: Romance, Ficção Científica, Técnico), preenchimento obrigatório.  

- **Saída:** Confirmação de registro bem-sucedido ou mensagem de erro em caso de preenchimento inadequado.

## 3. Fluxo Principal  
1. [O usuário acessa a página de cadastro.]
2. [O sistema valida as permissões do usuário.]
3. [O usuário insere os dados: título, autor, editora, categoria.]
4. [O sistema valida as entradas.]
5. [Se as entradas forem válidas o livro é cadastrado e o sistema exibe uma mensagem de sucesso.]

## 4 Fluxos Alternativos  
### Erro de autenticação
1. [Se as permissões do usuário não incluírem o registro de livros.]  
2. [O sistema exibe uma mensagem de erro.]  
3. [O sistema retorna para a página inicial.]  

### Erro de validação
1. [Se as entradas não forem válidas(Título já cadastrado, Editora não encontrada, etc).]  
2. [O sistema exibe uma mensagem de erro.]  
3. [O sistema solicita que o usuário confira as informações.]  

