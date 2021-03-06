# Adonis API application

This is the boilerplate for creating an API server in AdonisJs, it comes pre-configured with.

1. Bodyparser
2. Authentication
3. CORS
4. Lucid ORM
5. Migrations and seeds

## Setup

Use the adonis command to install the blueprint

```bash
adonis new yardstick --api-only
```

or manually clone the repo and then run `npm install`.

### Migrations

Run the following command to run startup migrations.

```js
adonis migration:run
```

#####

#Criando a rede do Docker

```sh
docker network create --driver bridge postgres-network
```

#Instalando o Postgres no Docker

docker run --name adonis --network=postgres-network -e "POSTGRES_PASSWORD=admin" -p 5432:5432 -v /Users/marcus/DESENVOLVIMENTO/PostgreSQL:/var/lib/postgresql/data -d postgres

### Linux:

```sh
docker run --name adonis -e "POSTGRES_PASSWORD=admin" -p 5432:5432 -v /home/marcus/developer/PostgreSQL:/var/lib/postgresql/data -d postgres
```

### MacOS:

```sh
MacBook-Air-de-MARCUS:~ marcus\$ docker run --name adonis --network=postgres-network -e "POSTGRES_PASSWORD=admin" -p 5432:5432 -v /Users/marcus/DESENVOLVIMENTO/PostgreSQL:/var/lib/postgresql/data -d postgres

```

docker run --name adonis -e "POSTGRES_PASSWORD=admin" -p 5432:5432 -v /Users/marcus/DESENVOLVIMENTO/PostgreSQL:/var/lib/postgresql/data -d postgres

5488634f1b778bc4248ed6adf608809408cc758a0e5e494309bfd48afb19328c
MacBook-Air-de-MARCUS:~ marcus\$ docker exec -it adonis /bin/bash

#Instalando o PGAdmin

```sh
root@localhost:~# docker pull fenglc/pgadmin4
root@localhost:~# docker run --name my_pgadmin4 -p 5050:5050 -d fenglc/pgadmin4
```

root@localhost:~# echo "host all all 172.17.0.0/24 md5" >> /var/lib/postgresql/data/pg_hba.conf
root@localhost:~# su postgres
postgres@localhost:~# psql -c "alter user postgres with password 'postgres';"
postgres@localhost:~# psql -c 'select pg_reload_conf();'

IP: 172.17.0.1

```sh
docker run --name postgres-gonode3 --network=postgres-network -p 15432:80 -e "PGADMIN_DEFAULT_EMAIL=mpaulobr@gmail.com” -e "PGADMIN_DEFAULT_PASSWORD=admin” -d dpage/pgadmin4
```

Acessando a URL http://localhost:15432 aparecerá a tela para login no pgAdmin 4:

```js
npm install -g @adonisjs/cli
```

```js
adonis new gonode --api-only
```

Rodar o projeto

```js
Adonis serve --dev
```

---

#Instalando o ESLint

```sh
npm install -D eslint
```

#Configurando o ESLint

```sh
npx eslint --init
```

# Instalando a dependência do Postgres

```sh
npm i --save pg
```

---

# Criando um Controller (Http)

```sh
adonis make:controller User
```

# Listando as Rotas do Adonis

```sh
adonis route:list
```

┌────────┬─────────┬──────────────────────┬────────────┬────────┬────────┐
│ Route │ Verb(s) │ Handler │ Middleware │ Name │ Domain │
├────────┼─────────┼──────────────────────┼────────────┼────────┼────────┤
│ /users │ POST │ UserController.store │ │ /users │ │
└────────┴─────────┴──────────────────────┴────────────┴────────┴────────┘

# Efetuando o rollback das migrations

```sh
adonis migration:rollback
```

# Instalando o Módulo de e-mail do Adonis

```sh
npm install @adonisjs/mail
```

# Criando um model

### -m: migration, -c: controller

```sh
adonis make:model Project -m -c
```

```sh
adonis make:model Task -m -c
```
