# Лаб 6. Docker Compose

## Цель
Создать два стека многоконтейнерных приложений:

- **Flask + Redis** — веб-приложение со счётчиком входов;
- **Prometheus + Grafana** — система мониторинга.

## Задачи
- Разработать и собрать стек Flask + Redis, реализующий веб-счётчик посещений.
- Развернуть стек Prometheus + Grafana.
- Настроить сбор метрик с приложения Flask и их отображение в Grafana.
- Все исходники загрузить в репозиторий на GitHub.
- В качестве ответа прикрепить ссылку на репозиторий.

## Развёртывание

```bash
git clone https://github.com/Lil-P0ly/situ_devops-lab_06.git
docker compose -f ./flask_redis/docker-compose.yml up --build -d
docker compose -f ./monitoring/docker-compose.yml up --build -d
```

## Пример работы
