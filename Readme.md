<h1 align="center">
    <img alt="GoBarber" title="#delicinha" src="./src/assets/logo.svg" width="250px" />
</h1>

<p align="center">
  <a href="#projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#layout">Layout</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#executando">Executando</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#licença">Licença</a>
</p>
<br>


## 💻 Projeto

Esse projeto foi desenvolvido no treinamento Gostack 14 da [Rocketseat](https://rocketseat.com.br/) dirigido por [Diego Fernandes](https://github.com/diego3g), onde o intuito era criarmos uma api para rest para ser consumida tanto na web quanto mobile.

## 🎨 Layout
O Layout pode ser conferido nestes repositórios:

[Web Gobarber](https://github.com/fabricioig863/GoBarber-web)

[App Gobarber](https://github.com/fabricioig863/App-GoBarber)


## 💻 Tecnologias

- [Node.js](https://nodejs.org/en/)
- [TypeScript](https://www.typescriptlang.org/)
- [Express](https://expressjs.com/pt-br/)
- [Multer](https://github.com/expressjs/multer)
- [TypeORM](https://typeorm.io/#/)
- [JWT-token](https://jwt.io/)
- [uuid v4](https://github.com/thenativeweb/uuidv4/)
- [PostgreSQL](https://www.postgresql.org/)
- [Date-fns](https://date-fns.org/)
- [Jest](https://jestjs.io/)
- [SuperTest](https://github.com/visionmedia/supertest)
- [Husky](https://github.com/typicode/husky)
- [Commitlint](https://github.com/conventional-changelog/commitlint)
- [Commitizen](https://github.com/commitizen/cz-cli)
- [Eslint](https://eslint.org/)
- [Prettier](https://prettier.io/)
- [EditorConfig](https://editorconfig.org/)


## Executando

### Faça o clone do repositório
```bash
# Digite o comando abaixo para clonar o repositório
$ git clone https://github.com/fabricioig863/API-Gobarber.git
```

# Iniciando o Projeto

## Instale as dependências
```bash
$ yarn

# Faça uma cópia de '.env.example' para '.env'
# ela é definida com SUAS variáveis de ambiente.
# As variáveis aws não precisam ser preenchidas para o ambiente dev
$ cp .env.example .env

# Crie a instância do postgreSQL usando docker
$ docker run --name gobarber-postgres -e POSTGRES_USER = docker \
               -e POSTGRES_DB = gobarber -e POSTGRES_PASSWORD = docker \
               -p 5433: 5433 -d postgres

# Crie a instância do mongoDB usando docker
$ docker run --name gobarber-mongodb -p 27017: 27017 -d -t mongo

# Crie a instância do redis usando docker
$ docker run --name gobarber-redis -p 6379: 6379 -d -t redis: alpino

# Faça uma cópia de 'ormconfig.example.json' para 'ormconfig.json'
# e defina os valores, se eles não forem preenchidos,
# para conectar-se ao contêiner do banco de dados do docker
$ cp ormconfig.example.json ormconfig.json

# Assim que os serviços estiverem em execução, execute as migrações
$ yarn typeorm migration: run

# Para terminar, execute o serviço api
$ yarn dev: server
```


## Licença

Este projeto está sob a licença MIT. Consulte o [LICENSE](LICENSE.md) para obter detalhes.

Feito com ❣️ por Fabricio Ignacio de Espindola



