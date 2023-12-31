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

Utilize o comando abaixo para iniciar o container:

```bash
docker compose up -d
```

## Para acessar o container

Utilize o comando abaixo para acessar o container:

```bash
docker exec -it php-fpm zsh
```

## Utilizando o container

Foi adicionado o `zsh` para facilitar a utilização do container, junto de alguns plugins para melhorar a experiência.
Também foi adicionado o `composer` para facilitar a instalação de dependências, alem da CLI do `symfony`.
Alguns exemplos de comandos podem ser vistos abaixo.

Para ver a versão do PHP

```bash
php -v
```

Para ver os módulos do PHP

```bash
php -m
```

Para ver o `php.ini`

```bash
php --ini
```

Para ver a versão do Composer

```bash
composer -V
```

Para ver os comandos do Symfony

```bash
symfony
```

## Acessando no navegador

Temos um exemplo de `index.php` com um `phpinfo()` para testar o ambiente.
Acesse url: `http://localhost:8888`.
