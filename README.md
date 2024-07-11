# monitoring-018
Chronograf and Kapacitor

**Домашнее задание**
Установка и настройка TICK стека

**Цель:**
Установить и настроить Telegraf, Influxdb, Chronograf, Kapacitor.
Результатом выполнения данного ДЗ будет являться публичный репозиторий, в системе контроля версий (Github, Gitlab, etc.), в котором будет находиться Readme с описанием выполненных действий. Файлы конфигурации Telegraf, Influxdb, Chronograf, Kapacitor должны находиться в директории TICK-1.


Описание/Пошаговая инструкция выполнения домашнего задания:
На виртуальной машине установите любую open source CMS, которая включает в себя следующие компоненты: nginx, php-fpm, database (MySQL or Postgresql);
На этой же виртуальной машине установите Telegraf для сбора метрик со всех компонентов системы (начиная с VM и заканчивая DB);
На этой же или дополнительной виртуальной машине установите Influxdb, Chronograf, Kapacitor
Настройте отправку метрик в InfluxDB.
Создайте сводный дашборд с самыми на ваш взгляд важными графиками, которые позволяют оценить работоспостобность вашей CMS;
Настройте правила алертинга для черезмерного потребления ресурсов, падения компонентов CMS и 500х ошибок;


1. Установлен telegraf для сбора метрик. Настроены input и output плагины. Конфиг тут
2. Установлен kapacitor и настроен конфиг для подключения к influxDb.
3. Установлен Chronograf и подключен так же к influxDb.
4. Насроен dashboard с мониторингом для хостав в целом и компонентов работы CMS (nginx, mysql, http, system) и мониторинг системы в целом.

