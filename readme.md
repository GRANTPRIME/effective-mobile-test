## стек:

- Python 3.12 (http.server)
- Nginx (reverse proxy)
- Docker
- Docker Compose

## Архитектура:

- Пользователь обращается к nginx
- Nginx проксирует запрос в Docker-сети на backend
- Backend отвечает текстом


## Как запустить проект

1. Перейти в корень проекта: cd effective-mobile-test

2. Собрать и поднять контейнеры: docker-compose up --build -d

3. Проверить статус контейнеров: docker ps

## Как проверить результат

В браузере открыть: http://localhost

Увидеть: Hello from Effective Mobile!