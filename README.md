# SpeedyCar - Sistema simples de Registro de Carros

![GitHub repo size](https://img.shields.io/github/repo-size/savio-2-lopes/SpeedyCar)
![GitHub language count](https://img.shields.io/github/languages/count/savio-2-lopes/SpeedyCar)
![GitHub top language](https://img.shields.io/github/languages/top/savio-2-lopes/SpeedyCar)
![GitHub followers](https://img.shields.io/github/followers/savio-2-lopes?label=Follow&style=social)

<br>

<p align="center">
  <img src="./.github/gif.gif" width="100%" alt="Web">
</p>

## Observação

Necessário possuir Docker instalado na máquina para rodar Backend e Frontend. Caso tenha mysql rodando na máquina, recomendo desativa para evitar conflitos de portas.

<br>

## Tecnologias do Backend

Tecnologias e ferramentas utilizadas no desenvolvimento do Backend:

- [PHP 8.1.0](https://www.php.net/releases/8.1/en.php)
- [Docker](https://www.docker.com/)
- [Swooler](https://openswoole.com/)
- [MySQL](https://www.mysql.com/)

<br>

## Tecnologias do Frontend

Tecnologias e ferramentas utilizadas no desenvolvimento do Frontend:

- [PHP 8.1.0](https://www.php.net/releases/8.1/en.php)
- [Docker](https://www.docker.com/)
- [Apache 2](https://httpd.apache.org/)
- [Bootstrap 5.3.0](https://getbootstrap.com/docs/5.2)
- [sweetalert2](https://sweetalert2.github.io)
- [Jquery](https://jquery.com/)

<br>

### API endpoints

`GET /veiculos`

Retorna todos os veículos

---

`GET /veiculos/:id`

Retorna dado de um veículo com base no `id`

---

`GET /veiculos/find?q="`

Retorna os veículos de acordo com o termo passado parâmetro `q`

---

`PUT /veiculos/:id`

Atualiza dado de um veículo com base no `id`

---

`REMOVE /veiculos/:id`

Remove dado de um veículo com base no `id`

---
`POST /veiculos`

Adiciona um novo veículo

<br>

## Instalação Backend

```bash
# Backend presente na pasta backend
$ cd backend

# Rodando o servidor com docker
$ docker compose up --build

# Necessário criar o banco de dados System-Project.
# Para isso, na pasta teste-fullstack-php/backend/app/create-table.sql há o script sql create-table.sql.
# Para acessar o banco de dados do Docker, as credenciais são as seguintes:
$ user: root;
$ password: root;
$ db: System-Project-backend;

## A api estará rodando usando IP da máquina
$ http:<SEU_IP>:8000

```

## Instalação Frontend

```bash
# Frontend presente na pasta backend
$ cd backend

# Rodando o servidor com docker
$ docker compose up --build

## Acessar usando IP da máquina
$ http:<SEU_IP>

## Em Service/VehicleService.php trocar o valor da url http://localhost:8000/veiculos para http://<SEU_IP>:8000/veiculos 
# De
$ private static $url = "http://localhost:8000/veiculos";
# Para
$ private static $url = "http://<SEU_IP>:8000/veiculos";
```

<br>

## Autor

[![Github Badge](https://img.shields.io/badge/-Github-373737?style=flat&logo=Github&logoColor=white)](https://github.com/savio-2-lopes)
[![Instagram Badge](https://img.shields.io/badge/-Instagram-8a3ab9?style=flat&logo=instagram&logoColor=white)](https://www.instagram.com/savioaugulopes/)
[![LinkedIn Badge](https://img.shields.io/badge/-LinkedIn-blue?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/savio-lopes/)
[![Gmail Badge](https://img.shields.io/badge/-Gmail-c14438?style=flat&logo=gmail&logoColor=white)](mailto:savio.dev.lopes@gmail.com)

Feito com ❤️ por [Savio Lopes](https://www.linkedin.com/in/savio-lopes/)

---
