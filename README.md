# app-pt-devops-bot
бот 

база данных psql

база данных psql с репликацией


DOCKER

docker build -t bot-image ./bot

docker build -t db-image ./db

docker build -t db_repl-image ./db_repl

 docker-compose up -d 


Заметка ANSILBL Перед сборкой или скачиваем :

1. Сборка происходила на 2 машинах обе убунты 
    1. на 1 убунте был сам ansible  и  основная база данных и бот
    2. на 2 убунте была база данных репликация
2. рВ файле inventory  указано 3 хоста ,  но база данных и бот это один и тот же хост    
 
1. Сборка происходит :
    1. заходим в нужную директорию
    2. запускаем след команду
    
    ```jsx
    ansible-playbook -i inventory playbook_tg_bot.yml
    ```
