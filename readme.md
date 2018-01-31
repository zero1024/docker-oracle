

**Старт контейнера с инициализацией бд из backup**

`docker run -d -p 1521:1521 --name oracle -v /backup/export:/docker-entrypoint-initdb.d oracle`

**Проверка стартанул ли oracle**

`docker exec oracle lsnrctl status`

