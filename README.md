# Информационная система управления складом с применением методов ИИ (WarehouseAI WMS)

Репозиторий для разработки системы по ТЗ: веб‑приложение на ASP.NET (Razor Pages/Minimal API) с PostgreSQL и подсистемой ИИ для прогнозирования спроса,
оптимизации размещения и маршрутов комплектации, обнаружения аномалий и интеллектуальной аналитики.

**Статус:** инициализация проекта по ТЗ.  
**Язык ТЗ:** русский.  
**Ключевые технологии:** ASP.NET, PostgreSQL, Python (ML), Docker, Kubernetes (опционально), Message Broker (RabbitMQ), OpenAPI/Swagger.

## Структура репозитория

- `docs/` — документация (ТЗ, схемы, модели данных, диаграммы).
- `api/` — спецификация API (OpenAPI), примеры клиентов.
- `src/` — исходный код подсистем (web, services, ml, workers).
- `infrastructure/` — Docker Compose/Helm чарты, IaC (опционально).
- `data/` — каталоги данных (raw/interim/processed), по умолчанию пустые.
- `models/` — артефакты моделей (по умолчанию пусто).
- `tests/` — тесты (unit, integration, e2e, ML‑валидация).
- `scripts/` — утилиты и миграции БД.
- `.github/` — CI/CD (GitHub Actions).

## Быстрый старт (локально с Docker)

```bash
docker compose -f infrastructure/docker-compose.yml up -d
```

Детали — см. `docs/TZ.md`.