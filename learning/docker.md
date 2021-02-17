**Docker**

### Instalação

_Windows_

Docker é executado em ambiente linux, então para isso será necessário instalar o WSL2 da microsoft

### Instalação WSL2

- Siga a opção manual de instalação presente [aqui](https://docs.microsoft.com/pt-br/windows/wsl/install-win10)
- baixe o linux ubuntu na Microsoft store

**Exemplo de um arquivo dockerfile**

```bash
# Especifica a versão do node
FROM node:14.15.5

# Especifica a pasta onde a imagem será salva
WORKDIR /usr/src/clean-node-api

# Copia os arquivos de package.json para `.` raíz da pasta
COPY package.json .

# Executa o script baixando somente as dependências de produção
RUN yarn add --only=prod

# Copia a pasta dist para a pasta dist do nosso WORKDIR
COPY ./dist ./dist

# Define a porta da nossa imagem
EXPOSE 5000

# Executa o script iniciando nosso servidor
CMD yarn start
```

### Scripts

Aqui alguns scripts úteis

```bash
# Exibe todo os containers em execução no momento
$ docker ps

# Exibe todos os containers
$ docker ps -a

# Para a execução de um container
# As 3 primeiras letras do id são o suficiente
# rm: remover
$ docker container rm <id>

# Para a execução de todos os containers de uma só vez
$ docker container prune

# Exibir imagens
# Flag -a: all
$ docker images -a

# Remover images
$ docker image rm <id>

# Gerar imagens e containers a partir do arquivo docker file
$ docker build -t clean-node-api <path_dockerfile>

# Exemplo: caso seu arquivo dockerfile estejá na raíz
$ docker build -t clean-node-api .

# Executa uma imagem de forma iterativa e abre no shell
$ docker run -it <your_image> sh

# Executa uma imagem em uma determinada porta
$ docker run -p 5000:5000 <your_image>
```
