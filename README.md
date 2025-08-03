

### Hexlet tests and linter status:
[![Actions Status](https://github.com/zhukata/devops-for-programmers-project-74/actions/workflows/hexlet-check.yml/badge.svg)](https://github.com/zhukata/devops-for-programmers-project-74/actions)

### Main tests status:
[![Actions Status](https://github.com/zhukata/devops-for-programmers-project-74/actions/workflows/push.yml/badge.svg)](https://github.com/zhukata/devops-for-programmers-project-74/actions)

# DevOps for Programmers 

JavaScript Fastify Blog - веб-приложение для ведения блога на Node.js с использованием Fastify.

## Требования к системе

- Docker и Docker Compose
- Node.js 20.x (для локальной разработки)
- PostgreSQL (для продакшена)

## Docker Hub образ

Образ доступен по адресу: `zhukata/devops-for-programmers-project-74`

## Инструкции для запуска

### Разработка
```bash
make dev
```

### Запуск тестов
```bash
make ci
```

### Переменные окружения

Создайте файл `.env` на основе `.env.example`:
```bash
cp app/.env.example .env
```

Основные переменные:
- `DATABASE_HOST` - хост базы данных
- `DATABASE_NAME` - имя базы данных
- `DATABASE_USERNAME` - пользователь базы данных
- `DATABASE_PASSWORD` - пароль базы данных

## Тесты

Тесты запускаются автоматически в CI/CD pipeline. Для локального запуска:

```bash
make ci
```