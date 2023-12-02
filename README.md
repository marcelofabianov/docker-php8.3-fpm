# PHP 8.3 (fpm)

Ambiente docker para se trabalhar com PHP 8.3 (fpm).

## Extensões

Algumas extensões já estão instaladas, mas você pode adicionar mais no arquivo `_docker/php-fpm/Dockerfile`.

- bcmath
- intl
- opcache
- mbstring
- soap
- redis
- apcu
- xdebug
- swoole
- pgsql
- pdo_pgsql

## Requisitos

Recomendo ter em seu ambiente:

- Docker 24+
- Docker Compose 2.23+

## Para iniciar

Utilize o comando abaixo para iniciar o ambiente:

```bash
docker compose up -d
```

## Para acessar o container

```bash
docker exec -it php-fpm zsh
```
