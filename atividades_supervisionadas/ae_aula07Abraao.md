# Atividade Extraordinária - Aula 07

## Técnicas para Especificação de Requisitos

As técnicas de especificação de requisitos são ferramentas importantes para descrever de maneira clara e compreensível as necessidades dos usuários, além de garantir que os desenvolvedores compreendam as funcionalidades a serem implementadas. A seguir, apresento duas técnicas comuns de especificação de requisitos, suas aplicações e as vantagens e desvantagens de cada uma.

### 1. Histórias de Usuário

#### Descrição:
As **histórias de usuário** são uma técnica amplamente utilizada em metodologias ágeis, como Scrum e Kanban. Elas descrevem as funcionalidades do sistema do ponto de vista do usuário, enfatizando o que o usuário deseja fazer com o sistema e o valor que isso traz para ele.

Uma história de usuário geralmente segue o formato:
- **Como [tipo de usuário],**  
- **Quero [funcionalidade],**  
- **Para que [benefício].**

#### Cenários em que são aplicáveis:
- **Desenvolvimento ágil de software:** Histórias de usuário são ideais quando se deseja uma forma simples e objetiva de capturar requisitos de maneira incremental.
- **Interação direta com o usuário:** Quando há necessidade de um entendimento claro das necessidades dos usuários finais e a comunicação precisa ser simples e eficaz.

#### Vantagens:
- **Simplicidade:** As histórias de usuário são fáceis de entender e comunicam rapidamente as necessidades do usuário de forma acessível a todas as partes envolvidas (desenvolvedores, designers, clientes).
- **Flexibilidade:** Facilitam ajustes rápidos no desenvolvimento do sistema, pois são orientadas a entregas incrementais.
- **Foco no valor:** Ao focar no benefício para o usuário, a técnica ajuda a manter o sistema alinhado com as expectativas reais dos usuários.

#### Desvantagens:
- **Falta de detalhes:** Histórias de usuário, por sua natureza, podem ser vagas em termos de requisitos técnicos, o que pode gerar ambiguidade e necessidade de esclarecimentos contínuos.
- **Possível falta de cobertura completa:** Como não cobrem todos os aspectos do sistema, pode ser necessário complementar com outras técnicas para uma especificação mais completa.

### 2. Casos de Uso

#### Descrição:
Os **casos de uso** são uma técnica de especificação que descreve como os usuários interagem com o sistema, especificando o comportamento do sistema a partir da perspectiva do usuário. Cada caso de uso foca em um cenário específico de interação e descreve passo a passo como o sistema deve responder.

Os casos de uso geralmente incluem:
- **Atores:** Quem interage com o sistema (usuários ou outros sistemas).
- **Objetivo:** O que o ator deseja alcançar.
- **Fluxo principal:** Os passos que o ator segue para alcançar seu objetivo.
- **Fluxos alternativos:** As variações no processo ou exceções.

#### Cenários em que são aplicáveis:
- **Sistemas complexos:** Casos de uso são ideais para sistemas que envolvem múltiplas interações e onde as variações nos fluxos de trabalho são significativas.
- **Documentação formal:** Quando a documentação precisa ser detalhada e estruturada, como em projetos grandes e com requisitos complexos.

#### Vantagens:
- **Completude:** Os casos de uso fornecem uma descrição detalhada de como os usuários devem interagir com o sistema, cobrindo vários cenários possíveis.
- **Clareza na comunicação:** São eficazes para comunicar os requisitos entre desenvolvedores, analistas e clientes, especialmente quando as interações do sistema precisam ser detalhadas.
- **Identificação de exceções:** Permitem o mapeamento de fluxos alternativos e exceções, o que é útil para garantir que todos os cenários sejam considerados.

#### Desvantagens:
- **Complexidade:** Para sistemas simples, a técnica pode ser excessivamente detalhada e difícil de gerenciar.
- **Dificuldade de manutenção:** Quando os requisitos mudam com frequência, manter os casos de uso atualizados pode ser desafiador, especialmente se houver muitas variações no comportamento do sistema.

---

## Especificação dos Requisitos

Com base no cenário que meu grupo é responsável pela modelagem, especificarei dois requisitos utilizando técnicas diferentes.

### Requisito A – Utilizando Histórias de Usuário

**Requisito:** O sistema deve oferecer um mecanismo de autentificação para garantir que os vendedores sejam legítimos e reduzir o risco de fraude.

**História de Usuário:**
- **Como** vendedor no sistema de marketplace,  
- **Quero** autenticar minha identidade de forma segura,  
- **Para que** o sistema garanta que sou um vendedor legítimo e ajude a reduzir o risco de fraude.

### Requisito B – Utilizando Casos de Uso

**Requisito:** A plataforma deve possibilitar a realização de pagamentos utilizando criptomoedas e outras formas de pagamento descentralizadas.

**Caso de Uso:**
- **Atores:** Usuário (comprador), Sistema, Processador de pagamento (plataforma de criptomoedas).
- **Objetivo:** Realizar pagamentos utilizando criptomoedas ou outras formas de pagamento descentralizadas.
- **Fluxo Principal:**
  1. O comprador acessa a página de pagamento da plataforma.
  2. O sistema oferece opções de pagamento, incluindo criptomoedas e formas descentralizadas.
  3. O comprador escolhe a forma de pagamento desejada (por exemplo, Bitcoin, Ethereum, etc.).
  4. O sistema processa o pagamento através da plataforma de pagamento descentralizada.
  5. O comprador recebe a confirmação de pagamento e a transação é finalizada.
- **Fluxos Alternativos:**
  1. Se a transação com criptomoeda falhar, o sistema oferece opções alternativas de pagamento descentralizado.
  2. Se o comprador não possuir criptomoeda suficiente, o sistema avisa o comprador e permite a escolha de outra forma de pagamento.

---

## Referências

- [ACERTBR - Técnicas de Elicitação de Requisitos](https://acertbr.com.br/tecnicas-de-elicitacao-de-requisitos/)
- [UNISINOS - Técnicas de Elicitação de Requisitos](https://unisinos.br/repositoriocanvas/Eng_Requisitos/html_Eng_Requisitos_tec_elicitacao/index.html)
- [UFSC - Guia de Técnicas de Elicitação de Requisitos](https://retraining.inf.ufsc.br/guia/app/classificacoes/tecnicas-de-elicitacao-de-requisitos)

---
