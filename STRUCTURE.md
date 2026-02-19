
# 📄 STRUCTURE.md


---

## Начало работы


Эти инструкции помогут вам пройти этап начальной загрузки при создании и развертывании примеров контейнеризированных приложений с помощью Docker и Docker Compose.


---

## Предварительные условия

✔ Убедитесь, что у вас установлены Docker и Docker Compose.     
✔ На Windows и MacOS: установите Docker Desktop   
✔ Linux: установите Docker и Docker Compose  


### Пример запуска

Корневой каталог каждого примера содержит файл compose.yaml, описывающий конфигурацию компонентов сервиса. Все примеры можно запустить в локальной среде, перейдя в корневой каталог каждого из них и выполнив команду:

```console
docker compose up -d
```

```console
docker build .
```

```console
docker run .
```

Проверьте файл `README.md` каждого примера, чтобы получить более подробную информацию о структуре и ожидаемом результате.
Чтобы остановить и удалить все контейнеры приложения-примера, выполните команду:

```console
docker compose down
```

```console
docker stop .
```
   
---   

## Production Dockerfile (с подробным объяснением)   

- [`Node.js`]() - Production, Multi-stage, non-root
- [`Python`]() - FastAPI / Django, Gunicorn
- [`Java`]() - Spring Boot, Multi-stage, JAR
- [`Go`]() - минимальный production
- [`Nginx`]() - frontend build + serve
- [`PHP`]() - Laravel + FPM
- [`PostgreSQL`]() - кастомный PostgreSQL (Автоматический init при первом запуске.)
- [`Redis`]() - Redis с конфигом
- [`Rust`]() - Rust multi-stage
- [`Universal template`]() - универсальный шаблон под debian
- [`Node.js + Prisma + Alpine + Healthcheck`]()
- [`Python + Poetry + Multi-stage`]()
- [`Java + Gradle + Layered JAR`]()
- [`Go + distroless`]()
- [`ASP.NET Core (Production)`]()
- [`Ruby on Rails`]()
- [`C++ + Multi-stage`]()
- [`Alpine + Cron Job container`]()
- [`Terraform container`]()
- [`Ansible automation container`]()
- [`Kafka Client container`]()
- [`Alpine Debug image`]()
- [`Multi-arch build example`]()
- [`React + Nginx + Gzip config`]()
- [`PostgreSQL + custom extensions`]()
- [`MongoDB custom init`]()
- [`Python Celery Worker`]()
- [`Nginx reverse proxy secure`]()
- [`Generic hardened base template`]()
- [``]()
