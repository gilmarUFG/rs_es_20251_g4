
## **1. Técnicas para Especificação de Requisitos**

### **Casos de Uso**

Casos de uso descrevem as interações entre usuários (atores) e o sistema para alcançar um determinado objetivo. Cada caso de uso mostra um fluxo de eventos, incluindo possíveis variações e exceções.

Usada principalmente em sistemas interativos, como plataformas web ou aplicações que exigem interação do usuário com diversas funcionalidades. Muito útil para entender como o usuário vai usar o sistema.

**Vantagens:**
- Fácil de entender por usuários não técnicos.
- Ajuda a identificar os atores e suas interações com o sistema.
- Facilita a transição para o design do sistema.

**Desvantagens:**
- Pode se tornar extenso em sistemas complexos.
- Não detalha requisitos não-funcionais (ex: segurança, desempenho).

---

### **Especificação por Requisitos Não Funcionais**

Essa técnica foca nas qualidades e restrições do sistema, como segurança, desempenho, confiabilidade, escalabilidade, etc. Os requisitos não funcionais geralmente são documentados em formato textual ou em tabelas.

Indicada quando o sistema precisa atender critérios de qualidade específicos, como em sistemas bancários, blockchain, ou sistemas críticos. Essencial quando a forma como o sistema faz algo é tão importante quanto o que ele faz.

**Vantagens:**
- Especifica claramente restrições e metas de qualidade.
- Ajuda no planejamento de testes e validação.
- Fundamental para sistemas onde segurança, desempenho e confiabilidade são críticos.

**Desvantagens:**
- Pode ser difícil de medir ou testar sem critérios claros.
- Muitas vezes subestimada ou mal documentada.

---

## **2. Especificação dos Requisitos**

### **Requisito: O sistema deve fornecer interoperabilidade entre diferentes blockchains.**

**Técnica aplicada: Casos de Uso**

**Caso de Uso: Interoperabilidade Blockchain**

- **Ator:** Desenvolvedor de aplicações (ou administrador da plataforma)
- **Objetivo:** Conectar e realizar transações entre diferentes blockchains (ex: Ethereum e Binance Smart Chain)
- **Pré-condição:** O usuário deve estar autenticado como administrador ou desenvolvedor autorizado.
- **Fluxo principal:**
  1. O ator acessa o painel de integração da plataforma.
  2. Seleciona as blockchains que deseja operar.
  3. A plataforma estabelece uma conexão segura com as redes selecionadas.
  4. O ator realiza uma transação de teste entre as blockchains.
  5. O sistema confirma a interoperabilidade com sucesso.
- **Fluxos alternativos:**
  - 3a. Falha na conexão: o sistema notifica o erro e oferece alternativas de diagnóstico.
  - 4a. Transação de teste falha: logs são gerados e o suporte técnico é notificado.
- **Pós-condição:** A interoperabilidade está habilitada entre as redes selecionadas.

---

### **Requisito: A plataforma deve garantir transações seguras e transparentes usando tecnologia blockchain.**

**Técnica aplicada: Requisitos Não Funcionais**

| Requisito Não Funcional | Descrição |
|--------------------------|-----------|
| **Segurança** | Todas as transações devem ser assinadas digitalmente usando chaves criptográficas (por exemplo, ECDSA). Dados sensíveis devem ser armazenados fora da blockchain com criptografia AES-256. |
| **Transparência** | Todas as transações devem ser registradas publicamente em blockchains públicas ou permissionadas acessíveis, garantindo imutabilidade e rastreabilidade. |
| **Confiabilidade** | A plataforma deve ter disponibilidade mínima de 99.9%, com redundância de nós para manter integridade em caso de falhas. |
| **Auditabilidade** | O sistema deve fornecer um log auditável de cada transação com timestamp, ID de transação e hash de verificação. |
