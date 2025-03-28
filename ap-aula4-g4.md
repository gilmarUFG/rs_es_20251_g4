# Requisito Funcional: RF004 - Cadastro de Livros

## 1. Descrição

O requisito funcional RF004 especifica que o sistema deve possibilitar o registro de livros, incluindo informações essenciais como título, autor, editora e categoria. Este requisito tem como objetivo garantir que os usuários possam adicionar livros ao catálogo de maneira padronizada e organizada. O sistema deve realizar validações para garantir que os dados inseridos sejam corretos e consistentes, evitando erros e registros duplicados.

## 2. Identificação das Fontes

As fontes para elicitação deste requisito incluem:

- **Bibliotecário**: Responsável pelo processo de registro e gerenciamento de livros no sistema.
- **Administrador do Sistema**: Usuário com permissão para configurar e administrar o sistema, incluindo permissões para o cadastro de livros.
- **Funcionário Responsável pelo Cadastro**: Pessoa que realiza o cadastro físico dos livros, com foco em inserir dados corretamente no sistema.

## 3. Técnicas de Elicitação de Requisitos

Durante o processo de elicitação, utilizam-se as seguintes técnicas para capturar os requisitos de forma precisa:

- **Entrevistas com Bibliotecários**: Condução de entrevistas para entender as necessidades e exigências quanto ao processo de cadastro, especialmente sobre as categorias de livros e os formatos dos dados.
- **Workshops**: Realização de workshops com stakeholders, incluindo administradores e bibliotecários, para alinhar as expectativas e definir os detalhes operacionais do sistema.
- **Prototipagem de Interfaces**: Apresentação de protótipos de telas de cadastro de livros para que os usuários possam visualizar e fornecer feedback sobre a interface e as funcionalidades esperadas.
- **Análise de Documentos Existentes**: Análise de sistemas de catalogação anteriores para entender como o cadastro de livros é realizado e identificar possíveis melhorias.
- **Questionários**: Aplicação de questionários para obter informações sobre as expectativas dos usuários finais em relação à funcionalidade de cadastro de livros.

## 4. Detalhamento do Requisito

### 4.1 Atores

- **Usuário com Permissão de Cadastro**: Este é o ator primário do processo, podendo ser um bibliotecário ou um administrador do sistema. Esses usuários têm a permissão necessária para realizar o cadastro de livros no sistema.

### 4.2 Entradas

O usuário deve fornecer as seguintes informações obrigatórias para o registro de um livro:

- **Título**: Nome do livro, que é um campo obrigatório. O sistema deve garantir que o título não seja duplicado no banco de dados.
- **Autor**: Nome(s) do(s) autor(es), sendo um campo obrigatório. O sistema deve permitir múltiplos autores, separados por vírgulas.
- **Editora**: Nome da editora responsável pela publicação do livro. Este campo também é obrigatório e, caso a editora não exista no banco de dados, o sistema deve permitir o cadastro de uma nova editora.
- **Categoria**: Classificação do livro (ex.: Romance, Ficção Científica, Técnico). A categoria é obrigatória e deve ser selecionada a partir de um conjunto predefinido de categorias ou permitida a adição de novas categorias, caso o usuário tenha permissão.

### 4.3 Saídas

- **Confirmação de Cadastro**: O sistema exibirá uma mensagem de sucesso caso o livro seja registrado corretamente.
- **Mensagem de Erro**: Caso algum dado esteja incorreto ou inválido (por exemplo, título duplicado, editora não encontrada), o sistema exibirá uma mensagem de erro indicando qual campo precisa ser corrigido.

### 4.4 Validações

- **Título**: O sistema valida se o título já está cadastrado. Caso positivo, o usuário será informado sobre a duplicidade.
- **Autor**: O campo autor deve aceitar múltiplos autores separados por vírgulas.
- **Editora**: O sistema valida se a editora existe no banco de dados. Se não existir, o sistema permite ao usuário cadastrar uma nova editora.
- **Categoria**: O sistema valida se a categoria informada é válida. Caso contrário, o sistema informa um erro.

## 5. Fluxo Principal

O fluxo principal descreve as etapas do processo de cadastro de um livro:

1. O **usuário** acessa a página de cadastro de livros no sistema.
2. O **sistema** valida as permissões do usuário (somente bibliotecários ou administradores podem cadastrar livros).
3. O **usuário** insere os dados obrigatórios: título, autor, editora e categoria.
4. O **sistema** realiza as validações das entradas, verificando duplicidade de título, existência de editora e validade da categoria.
5. Se as entradas forem válidas, o **sistema** registra o livro e exibe uma mensagem de sucesso: "Livro cadastrado com sucesso."

## 6. Fluxos Alternativos

### 6.1 Erro de Autenticação

1. Se o **usuário** não possuir permissão para cadastrar livros, o **sistema** exibirá uma mensagem de erro: "Você não tem permissão para cadastrar livros."
2. O **sistema** retornará à página inicial ou à página de login.

### 6.2 Erro de Validação

1. Se as entradas não forem válidas (por exemplo, título duplicado, editora não encontrada, categoria inválida):
   - O **sistema** exibirá uma mensagem de erro específica para cada campo inválido (ex.: "Título já cadastrado", "Editora não encontrada", "Categoria inválida").
   - O **sistema** solicitará que o **usuário** corrija os dados e tente novamente.

### 6.3 Erro de Sistema

1. Caso ocorra uma falha inesperada, como erro de conexão com o banco de dados:
   - O **sistema** exibirá uma mensagem genérica: "Ocorreu um erro ao tentar cadastrar o livro. Tente novamente mais tarde."
   - O **sistema** registrará o erro para análise posterior e não permitirá o cadastro até que o problema seja resolvido.

## 7. Considerações Finais

- **Segurança**: Apenas usuários com as permissões adequadas (como bibliotecários e administradores) devem poder cadastrar livros no sistema.
- **Desempenho**: O sistema deve ser eficiente ao processar grandes volumes de registros de livros, sem comprometer a performance.
- **Usabilidade**: A interface de cadastro deve ser intuitiva, proporcionando uma experiência de usuário fluída, com validações claras e feedback adequado.

---

Este documento descreve o processo de cadastro de livros, alinhado com as melhores práticas de Engenharia de Requisitos, garantindo que o sistema atenda às necessidades dos usuários de forma eficiente e confiável.
