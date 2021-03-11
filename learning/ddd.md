**Domain Driven Design**

<br />
  A base do DDD diz que o desenvolvimento de uma solução de software deve ser feito respeitando-se algumas camadas para a
organização da solução:

<br />

 - **Camada de Apresentação**: é a famosa "interface com o usuário". Essa camada é a responsável por apresentear as informações ao
usuário e interpretar os comandos do mesmo
 - **Camada de Aplicação**: essa deve ser uma fina camada que coordena as atividades da aplição. Aqui não deve haver lógica de negócio envolvida.
 - **Camada de Domínio**: essa é a camada que possui as informações do domínio e deve ser considerada o "coração" da solução.
 - **Camada de Infraestrutura**: essa camada deve atuar como uma camada de suporte para as demais. Uma provedora da interligação entre as camadas, implementar a persistência dos objetos do negócio e conter as bilbiotecas de suporte.

### Camadas

- **Domain:** Interfaces da regra de negocio
- **Data:**: Protocolos e casos de uso relacionado ao banco de dados
- **Infra:** Implementações e adaptadores de bibliotecas
- **Presentation:** controlador de requisições, respostas e validações
- **Main:** Composição de todas as camadas

### Relacionamento

- **Domain:** -> Não conhece ninguém
- **Data** -> **Domain**
- **Presentation** -> **Domain**
- **Infra** -> **Data**
- **Main** -> Conhece todas as camadas
