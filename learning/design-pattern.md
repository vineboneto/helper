**Princípios comuns de design**

Há diversos princípios comuns de design, que, assim como os design patterns, se tornaram boas práticas através dos anos e ajudaram a formar uma fundação no qual o nível empresarial e software de fácil manutenção podem ser construídos. Abaixo, segue um resumo dos princípios mais conhecidos:

> ### Keep It Simple Stupid (KISS)
_Mantenha Isto Estupidamente Simples_
<br />

Um problema comum em programação de software é a necessidade de complicar demais a solução. O objetivo do princípio KISS é manter o código simples, mas não simplista, assim evitando complexidade desnecessária.

> ### Don’t Repeat Yourself (DRY)
_Não Repita Você Mesmo_
<br />
O princípio do DRY é evitar a repetição de qualquer parte do sistema abstraindo as coisas que são comuns entre si e colocá-las em um lugar único. Esse princípio não se preocupa somente com o código, mas qualquer lógica que está duplicada no sistema.

> ### Tell, Don’t Ask
_Fale, não pergunte_
<br />
O principio Tell, Don’t Ask está estreitamente alinhado com o encapsulamento e a atribuição de responsabilidades para as suas classes corretas. O princípio afirma que você deve dizer aos objetos quais ações você quer que eles realizem, ao invés de fazer perguntas sobre o estado do objeto e então tomar uma decisão por si próprio em cima da ação que você quer realizar. Isso ajuda a alinhar as responsabilidades e evitar o forte acoplamento entre as classes.

>### You Ain’t Gonna Need It (YAGNI)
_Você Não Vai precisar Disso_
<br />
O princípio YAGNI se refere a necessidade de adicionar somente as funcionalidades que são necessárias para a aplicação e deixar de lado qualquer tentação de adicionar outras funcionalidades que você acha que precisa. A metodologia de projeto que adere ao YAGNI é a test-driven development (TDD) – desenvolvimento orientado a testes. TDD se baseia na escrita de testes que comprovam a funcionalidade do sistema e então escrevem somente o codigo para obter êxito no teste.

> ### Separation Of Concerns (SoC)
_Separação de Responsabilidades_
<br />
SoC é o processo de dissecação de uma parte de software em distintas características que encapsulam um único comportamento e dados que podem ser utilizados por outras classes. Geralmente, a responsabilidade representa uma características ou comportamento da classe. O ato de separar um programa em discretas responsabilidades aumenta significativamente a reutilização de código, manutenção e testabilidade.

> ### Decorator
_Decorador_
<br />
Decorator, wrapper , é um padrão de projeto de software que permite adicionar um comportamento a um objeto já existente em tempo de execução, ou seja, agrega dinamicamente responsabilidades adicionais a um objeto.[1] Decorators oferecem uma alternativa flexível ao uso de herança para estender uma funcionalidade, com isso adiciona-se uma responsabilidade ao objeto e não à classe.

