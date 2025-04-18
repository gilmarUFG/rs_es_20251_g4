# Atividade Prática 1 - Aula 2 - 13/03/2025

### Discentes:
* Abraão Santiago Moreira (202201679);
* Felipe Moreira Silva (202201689);
* Frederico Garcez Rodrigues (202201690);
* Joseppe Pedro Cunha Fellini (202300194);
* Mauro Sérgio do Nascimento Júnior (202204842);

### Contexto
A proposta de sistema é para o desenvolvimento de um software de gerenciamento de reservas de livros em uma biblioteca escolar, com o objetivo de otimizar o processo de empréstimo e devolução de livros, garantindo que o controle seja eficiente e acessível para todos os envolvidos (bibliotecários, alunos, professores e diretores). Este sistema visa melhorar a organização e a experiência do usuário, além de proporcionar maior agilidade e precisão na gestão dos recursos bibliográficos.

### Requisitos Funcionais
**RF001** - O software deve possibilitar a busca de qualquer tipo de título. A busca deve ser abrangente e considerar: nome do livro, autor, editora, edição, categoria e até mesmo descrição.

**RF002** - O software deve possibilitar ao aluno visualizar todos os livros mesmo aqueles que já estão reservados, porém informando-o que o livro visualizado já foi reservado sem informar quem o reservou.

**RF003** - O software deve possibilitar o pagamento de multas pendentes para os locadores de livros, assim como a anexação de pagamentos presenciais.

**RF004** - O software deve possibilitar o registro de livros com título, autor, editora, categoria.

**RF005** - O software deve possibilitar autenticação para identificação de ação de locadores e administradores.

### Requisitos Não Funcionais:
**RNF001** - O sistema deve funcionar de forma consistentemente em dispositivos móveis.

**RNF002** - O sistema deve ser capaz de lidar com diferentes sistemas operacionais, como Windows, macOS e Linux sem necessidade de modificação.

**RNF003** - O sistema deve possuir uma interface intuitiva e acessível para diferentes perfis de usuários.

**RNF004** - O sistema deve manter a segurança dos dados de acordo com regras de _compliance_ vigentes.

**RNF005** - O sistema deve ser tolerante a falhas, conseguindo manter os dados mesmo em contextos adversos de hardware ou software, minimizando o _downtime_.

### Regras de Negócio:
**RN001** - Alunos com reservas pendentes ficam impossibilitados de realizar matrícula.

**RN002** - Após tempo limite de reserva será cobrado uma multa que será cobrada por cada dia de atraso.

**RN003** - Alunos só podem renovar a reserva de um único livro 4 vezes consecutivas.

**RN004** - Livros de acervo restrito só podem ser reservados por grupos de Professores e alunos com autorização prévia.

**RN005** - Os livros devem ser devolvidos dentro de um prazo estipulado (15 dias por exemplo).
