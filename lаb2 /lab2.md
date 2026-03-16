University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FTMI](https://ftmi.itmo.ru/)\
Course: [Введение в веб технологии](https://itmo-ict-faculty.github.io/introduction-in-web-tech/)\
Year: 2025/2026\
Group: U4125\
Author: Nikitina Valeriya Sergeevna\
Lab: Lab2\
Date of create: 16.03.2026\
Date of finished: 16.03.2026


1) Скопировала файлы из первой лабораторной (app.py, requirements.txt, Dockerfile) в новый репозиторий [devops-lab2-nikitina](https://github.com/vsnikitina2001-ops/devops-lab2-nikitina/tree/main).
Создала аккаунт на Docker Hub. Создала новый репозиторий на Docker Hub для образа.


Настройка GitHub Actions:

Создать папку .github/workflows/ в корне проекта
Создать файл docker-build.yml с пайплайном, который должен:
Запускаться при пуше в main ветку
Использовать Ubuntu как runner
Выполнять checkout кода
Настраивать Docker Buildx
Логиниться в Docker Hub используя секреты
Собирать и пушить образ с тегом username/my-flask-app:latest
Добавлять шаг деплоя (можно просто echo сообщение)
Настройка секретов:

В настройках GitHub репозитория добавить секреты:
DOCKER_USERNAME - ваш логин на Docker Hub
DOCKER_PASSWORD - ваш пароль или токен доступа Docker Hub
Тестирование пайплайна:

Сделать коммит и пуш в main ветку
Проверить выполнение пайплайна в разделе Actions
Убедиться, что образ появился в Docker Hub
Проверить логи выполнения каждого шага
