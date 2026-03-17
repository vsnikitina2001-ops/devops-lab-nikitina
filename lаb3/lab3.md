University: [ITMO University](https://itmo.ru/ru/)\
Faculty: [FTMI](https://ftmi.itmo.ru/)\
Course: [Введение в веб технологии](https://itmo-ict-faculty.github.io/introduction-in-web-tech/)\
Year: 2025/2026\
Group: U4125\
Author: Nikitina Valeriya Sergeevna\
Lab: Lab3\
Date of create: 16.03.2026\
Date of finished: 16.03.2026


1) Создала папку prometheus для конфигурации.
Создала файл prometheus/prometheus.yml. Запустила Node Exporter.
![3.1.png](https://github.com/vsnikitina2001-ops/devops-lab-nikitina/blob/main/l%D0%B0b3/images3/3.1.png)
2) Запустила контейнер Node Exporter для сбора системных метрик.
Проверила работу: curl http://localhost:9100/metrics

3) Создала том для данных Prometheus:
Вышла на папку выше в консоли, убедилась что вы находитесь над уровнем папки prometheus. Запустила контейнер Prometheus.

4) Проверила работу: открыть http://localhost:9090 в браузере.

5) Создала том для данных Grafana.
Проверила работу: открыть http://localhost:3000 в браузере.

6) Проверила все контейнеры.
Открыла Prometheus и убедилась, что метрики собираются.
Создала несколько графиков для разных метрик (CPU, память, диск).
