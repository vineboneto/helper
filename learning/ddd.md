**Domain Driven Design**

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
