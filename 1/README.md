# Докер образ

Сборка:
```
docker build --no-cache -t access-control-api . 
```
Запуск:
```
docker run -p 8082:8082 
    -e MYSQL_HOST=host.docker.internal 
    -e MONGODB_HOST=host.docker.internal 
    -e RECOGNITION_MODEL_SERVICE_HOST=host.docker.internal 
    --rm access-control-api
```
