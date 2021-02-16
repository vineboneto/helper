# Bibliotecas

> **yarn**

- Gerência pacotes

```bash
$ yarn init -y
```

> **git-commit-msg-linter**

- Evita commits realizados com a formatação errada
- Commits devem ser realizados seguindo a seguinte formatação
  -Exemplo: `"chore: add yarn"`
- Tudo dever estar em minúsculo e o verbo deve estar no imperativo

```
$ yarn add git-commit-msg-linter -D
```

> **eslint**

- Verifica se o seu código está seguindo a formatação convencional e mais utilizada pelo js/ts
- Typescript precisa de muitos plugins para conseguir instalar o eslint. Acesse [aqui](https://github.com/standard/eslint-config-standard-with-typescript).

> **husky**

- Invalida tentativas de commit que não seguem as regras estabelecidas pelo eslint

```
$ yarn add husky -D
```

# Configurações de Bibliotecas

> **typescript**

- As configurações de compilação do typescript são armazenadas em um arquivo `.tsconfig.json`

```bash
{
  "compilerOptions": {
    "outDir": "./dist",
    "module": "commonjs",
    "target": "es2019",
    "esModuleInterop": true,
    "allowJs": true,
  }
}
```

- **outDir:** Pasta de produção
- **module:** Converter as importações/exportações para require/module.export. Versões suportadas pelos browsers
- **target:** versão javascript que o typescript será convertido
- **esModuleInterop:** converter módulos para commonjs
- **allowJs:** Se possuir arquivos de configuração no formato de javascript ao invés de json, incluirá no dist

> **eslint**

- As configurações do eslint são armazenadas em um arquivo `.eslintrc.json`

```bash
{
  {
  "extends": "standard-with-typescript",
  "parserOptions": {
    "project": "./tsconfig.json"
  }
}
```

- **extends:** estende a biblioteca utilizada pelo eslint
- **project:** apontamento para o arquivo configuração do typescript
