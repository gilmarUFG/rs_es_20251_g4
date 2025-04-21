# Técnicas para especificação

## 1.

### Prototipação

A simulação de comportamentos ou interfaces do sistema é uma boa forma de garantir o alinhamento das expectativas dos clientes com as ideias de implementação da equipe de desenvolvimento, uma vez que possibilita uma visão prévia de como o sistema funcionará, além de possuir um custo várias vezes menos que o de um produto propriamente dito. Dessa forma, problemas conceituais podem ser notados antes que sejam propagados pelo código do projeto final.

### Casos de Uso

O uso de diagramas de casos permite representar graficamente as ações que cada ator do sistema conseguirá realizar. Essa abordagem evidencia possíveis mal-entendidos em relação a permissões de acesso e responsabilidades.

![alt text](image.png)

## 2.

### Avaliações e comentários armazenados em blockchain para evitar manipulação.

**Técnica de especificação: Modelagem UML (Diagrama de Sequência)**
![alt text](image-1.png)

### A plataforma deve permitir que o usuário devolva um produto comprado e receba seu dinheiro na mesma forma do pagamento efetuado

**Técnica de especificação: História de usuário**

>**Como** usuário da plataforma  
**Eu quero** ter a opção de solicitar a devolução e reembolso  
**Para** exercer meu direito a arrependimento e reaver o dinheiro gasto na compra.
               
>**Cenário 1:**  Devolução efetivada  
**Dado que** recebi o produto há menos de 7 dias  
**E** comuniquei a plataforma sobre a devolução  
**Quando** a solicitação for aceita pela plataforma
**Então** a empresa fornecerá as instruções de envio do produto
**E** realizarei o envio dentro do prazo estabelecido.