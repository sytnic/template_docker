# Template project

- Docker
- PHP 7.4
- Apache
- MySQL 5.7.39
- Adminer

## Запуск Docker

Запуск контейнеров

    docker-compose build
    docker-compose up -d

> Проверка в браузере

    127.0.0.1:8080
    127.0.0.1:8080/adminer.php

> Вход в бд

    db, root, 123
    // берётся из docker-compose.yml

## Вход в контейнер, если необходимо

    cd /d E:\
    cd E:\Projects_greycrud\template_docker
    dir
    docker ps
    docker exec -it container_id bash 
    (не работает в GitBash, работает в cmd)

    # apt-get install nano

## Остановка контейнеров

    docker-compose stop