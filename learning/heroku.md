**Heroku**

Hospedagem de aplicativos

### Requerimento

Seu `package.json` deve possuir os seguintes scripts:

- `build` para construir seu aplicativo em produção
- `start` para executar o server da sua aplicação em produção

### Instalação

Em sua conta de heroku baixe o `cli` presente na aba `deploy` e instale-o

- Realize o login em heroku

```bash
# Habilita pull e push para o repositório do heroku
$ heroku login
```

- Vá para raiz de seu projeto e execute

```bash
# Caso já exista um repositório
$ heroku git:remote -a <your-repository-heroku>

# Caso seja um novo repositório
$ git init
$ heroku git:remote -a <your-repository-heroku>

# Exemplo
$ heroku git:remote -a my-api-node-ts

# Isso irá criar novos remotes associados ao repositório do heroku.
# Os mesmos podem ser visualizados com:
$ git remote -v
```

- Realizar deploy da aplicação

```bash
# Dessa forma é possível realizar pull e push para o repositório heroku. Exemplo:
$ git push heroku master
# ...Instalando dependências de produção,
# executando script build e
# então executando script start
```

Observações

```bash
# Em caso de erro abra a pasta raiz do seu projeto e tente:
$ heroku restart
```

### Configuração

Adicionar variáveis de ambiente

- Vá para aba `Settings`
- Localize `Config Vars`
- Adicione as variáveis de ambiente

```bash
# Exemplo
JWT_SECRET: ADS-9F8KF-ASJ2A0SDF8A0SKlsakjf.xcv0
MONGO_URL: <your_url_mongo_db_product>
```

[Como configura mongodb em produção](../db/mongodb.md#mongodb-altas)
