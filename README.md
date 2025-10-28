# Домашнее задание к занятию «Система мониторинга Prometheus»

**Студент:** Dudnikov Daniil  
**Рабочая станция:** dudnikov-daniil  
**ОС:** Ubuntu 24.04.3

---

## Задание 1: Установка Prometheus

### Выполненные действия:
- Создан пользователь `prometheus`
- Установлен Prometheus 2.51.0
- Настроены системные директории
- Создан systemd сервис с описанием "Prometheus Service Netology Lesson 9.4 - Dudnikov Daniil"
- Проверена работа службы

### Результат:
![Status Prometheus](screenshots/Задание%201.png)

---

## Задание 2: Установка Node Exporter

### Выполненные действия:
- Создан пользователь `node_exporter` 
- Установлен Node Exporter 1.8.1
- Создан systemd сервис с описанием "Node Exporter Netology Lesson 9.4 - Dudnikov Daniil"
- Проверена работа службы

### Результат:
![Status Node Exporter](screenshots/Задание%202.png)

---

## Задание 3: Подключение Node Exporter к Prometheus

### Выполненные действия:
- Обновлена конфигурация `prometheus.yml`
- Добавлен job для Node Exporter
- Перезапущен Prometheus
- Проверено подключение в веб-интерфейсе

### Результат:
**Конфигурация Prometheus:**
![Prometheus Configuration](screenshots/Задание%201.1.png)

**Цели мониторинга (2 эндпоинта):**
![Prometheus Targets](screenshots/Задание%202.1.png)

---

## Задание 4*: Установка Grafana

### Выполненные действия:
- Установлен Grafana через snap
- Настроен профиль пользователя
- Указаны ФИО "Dudnikov Daniil" в профиле

### Результат:
![Grafana Profile](screenshots/Задание%204.png)

---

## Задание 5*: Интеграция Grafana и Prometheus

### Выполненные действия:
- Добавлен источник данных Prometheus
- Импортирован дашборд Node Exporter
- Проверен сбор метрик

### Результат:
**Источник данных Prometheus:**
![Grafana Data Source](screenshots/Задание%205.1.png)

**Рабочий дашборд Node Exporter:**
![Grafana Dashboard](screenshots/Задание%205.2.png)

---

## Общий вывод

**Все компоненты системы мониторинга успешно установлены и интегрированы:**
- **Prometheus** - сбор метрик
- **Node Exporter** - системные метрики  
- **Grafana** - визуализация данных
- **Все службы работают корректно**

