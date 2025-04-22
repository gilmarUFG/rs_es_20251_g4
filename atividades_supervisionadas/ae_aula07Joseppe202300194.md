# Técnicas para Especificação de Requisitos

## 1. Técnicas de Especificação de Requisitos

### 1.1 Diagrama de Máquina de Estados

O Diagrama de Máquina de Estados é uma técnica de modelagem que representa os diferentes estados de um objeto e as transições entre esses estados. Esta técnica faz parte da UML e é útil para especificar comportamentos complexos e dependentes de estado.

**Cenários Aplicáveis:** Sistemas com comportamentos dependentes de estado, interfaces com múltiplos modos, protocolos de comunicação e sistemas de controle.

**Vantagens e Desvantagens:**

- **Vantagens:** Visualização clara dos estados possíveis, facilita a compreensão de comportamentos complexos, identifica todos os caminhos possíveis.
- **Desvantagens:** Complexo para sistemas com muitos estados, difícil de manter com mudanças frequentes, requer conhecimento de UML.

### 1.2 Prototipação

A Prototipação envolve a criação de uma versão preliminar do sistema para validar requisitos. Permite que usuários interajam com o protótipo e forneçam feedback antes da implementação completa.

**Cenários Aplicáveis:** Interfaces de usuário, requisitos ambíguos, sistemas com forte interação com usuários e validação de conceitos inovadores.

**Vantagens e Desvantagens:**

- **Vantagens:** Facilita a comunicação, permite validação antecipada, reduz riscos, identifica problemas de usabilidade.
- **Desvantagens:** Pode criar expectativas irrealistas, foco excessivo na interface, requer recursos adicionais, difícil representar requisitos não-funcionais.

## 2. Especificação de Requisitos para Plataforma de E-commerce com Blockchain

### 2.1 Requisito 1: Armazenamento Seguro de Cartões Bancários

#### **Técnica utilizada: Caso de Uso**

**Nome:** UC-001: Armazenar Informações de Cartão Bancário de Forma Segura

**Atores:** Usuário, Sistema de Pagamento, Sistema de Segurança

**Fluxo Principal:**

1. Sistema apresenta formulário para dados do cartão
2. Usuário preenche e seleciona "Salvar cartão"
3. Sistema valida, criptografa e armazena os dados
4. Sistema gera token e registra hash na blockchain
5. Sistema confirma ao usuário

**Fluxos Alternativos:**

- Dados inválidos: Sistema exibe erros, usuário corrige
- Falha na criptografia: Sistema registra erro e notifica usuário

**Requisitos Especiais:** Conformidade com PCI DSS, criptografia AES-256, registro de auditoria, detecção de fraude.

### 2.2 Requisito 2: Compatibilidade com Criptomoeda DogeCoin

#### **Técnica utilizada: História de Usuário**

**História Principal:**
**Como** cliente da plataforma, **quero** utilizar DogeCoin para pagamentos, **para que** possa aproveitar minhas criptomoedas de forma conveniente.

**Critérios de Aceitação:**

- Opção de pagamento com DogeCoin disponível no checkout
- Exibição do valor equivalente com base na cotação atual
- Geração de QR code para pagamento
- Verificação da transação na blockchain
- Notificação sobre status da transação
- Emissão de recibo digital

**Requisitos Técnicos:** Integração com API de cotação, monitoramento de transações na blockchain, mecanismo de reembolso, conformidade regulatória.
