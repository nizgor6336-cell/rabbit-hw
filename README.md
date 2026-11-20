# Домашнее задание к занятию «ELK»

**Выполнил:** Нижегородцева Ольга Сергеевна

---

## Задание 1. Elasticsearch

Установлен и запущен Elasticsearch в Docker. Параметр `cluster_name` изменен на нестандартный.

Скриншот команды `curl -X GET 'localhost:9200/_cluster/health?pretty'`:
![Задание 1](scr1.png)

---

## Задание 2. Kibana

Установлена и запущена Kibana. Через интерфейс Dev Tools выполнен запрос `GET /_cluster/health?pretty`.

Скриншот интерфейса Kibana:
![Задание 2](scr2.png)

---

## Задание 3. Logstash

Установлен и запущен Logstash и Nginx. С помощью Logstash настроена отправка access-лога Nginx в Elasticsearch. Логи успешно распарсены.

Скриншот логов Nginx в Kibana:
![Задание 3](scr3.png)

---

## Задание 4. Filebeat

Установлен и запущен Filebeat. Поставка логов Nginx переключена с Logstash на Filebeat. Логи успешно поступают в Elasticsearch.

Скриншот логов Nginx, отправленных через Filebeat:
![Задание 4](scr4.png)
