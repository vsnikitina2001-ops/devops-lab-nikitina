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

2) Cоздала папку .github/workflows/ в корне проекта& Создаkf файл docker-build.yml с пайплайном, который должен:
Запускаться при пуше в main ветку;
Использовать Ubuntu как runner;
Выполнять checkout кода;
Настраивать Docker Buildx;
Логиниться в Docker Hub используя секреты;
Собирать и пушить образ с тегом username/my-flask-app:latest;
Добавлять шаг деплоя (можно просто echo сообщение).

3) В настройках GitHub репозитория добавила секреты:
DOCKER_USERNAME - логин на Docker Hub
DOCKER_PASSWORD - пароль на Docker Hub

4) Сделала коммит и пуш. Проверила выполнение пайплайна в разделе Actions.
Образ появился в Docker Hub. Проверила логи выполнения каждого шага.

![1.1.png](https://github.com/vsnikitina2001-ops/devops-lab-nikitina/blob/main/lab1%20/images1/1.1.png)

