<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h3 align="center">
  Desafio 02: Conceitos do Node.js
</h3>

<p align="center">“Não espere para plantar, apenas tenha paciência para colher”!</blockquote>

## :rocket: Sobre o desafio

Esse é o primeiro desafio de NodeJS da turma 11 do GoStack. O desafio envolve a aplicação de todos os conhecimentos sobre conceitos de NodeJS vistos na segunda fase do curso.

Essa aplicação serve para armazenar repositórios do seu portfólio, permitindo a criação, listagem, atualização e remoção dos repositórios, e além disso, ainda permite que os repositórios possam receber "likes".

### Rotas da aplicação

- **`POST /repositories`**: A rota recebe `title`, `url` e `techs` dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo repositório, ele é armazenado dentro de um objeto no seguinte formato: `{ id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 }`;

- **`GET /repositories`**: Rota que lista todos os repositórios;

- **`PUT /repositories/:id`**: A rota altera apenas o `título`, a `url` e as `techs` do repositório que possui o `id` igual ao `id` presente nos parâmetros da rota;

- **`DELETE /repositories/:id`**: A rota deleta o repositório com o `id` presente nos parâmetros da rota;

- **`POST /repositories/:id/like`**: A rota aumenta o número de likes do repositório específico escolhido através do `id` presente nos parâmetros da rota;

### Tecnologias utilizadas

+ [Express](https://expressjs.com/pt-br/) 

+ [uuidv4](https://www.npmjs.com/package/uuidv4)

+ [Nodemon](https://www.npmjs.com/package/nodemon)

### Forma de utilizar

```sh
  git clone https://github.com/guilhermeaw/desafio-conceitos-node.git
  cd desafio-conceitos-node && yarn
```

##### Rodar o Projeto
```sh
  yarn dev
```

##### Rodar os testes

```sh
  yarn test
```

---
