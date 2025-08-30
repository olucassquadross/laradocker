# Laravel 12 com Docker

Este projeto utiliza Laravel 12, Docker, Nginx e MySQL.

## Como clonar o projeto

```sh
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
```

## Como rodar o projeto com Docker

1. **Certifique-se de que o Docker Desktop está instalado e em execução.**

2. **Construa e suba os containers:**

```sh
docker compose up --build
```

3. **Execute as migrations (opcional, se necessário):**

```sh
docker compose exec app php artisan migrate
```

4. **Acesse o projeto:**

Abra [http://localhost:8000](http://localhost:8000) no navegador.

## Estrutura dos containers

- **app**: PHP-FPM + Composer
- **webserver**: Nginx
- **db**: MySQL

## Editando o projeto

Você pode editar os arquivos do Laravel diretamente na pasta local. As alterações são refletidas automaticamente