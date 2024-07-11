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


1. Установлен telegraf для сбора метрик. Настроены input и output плагины. [Конфиг](https://github.com/Vladimir174/monitoring-018/blob/main/telegraf.conf)
2. Установлен kapacitor и настроен конфиг для подключения к influxDb. [Конфиг](https://github.com/Vladimir174/monitoring-018/blob/main/kapacitor.conf) 
3. Установлен Chronograf и подключен так же к influxDb.
   ![image](https://github.com/Vladimir174/monitoring-018/assets/40054398/22d808b3-7474-4bd5-840b-722302aa8877)

5. Насроен dashboard с мониторингом для хостав в целом и компонентов работы CMS (nginx, mysql, http, system) и мониторинг системы в целом.
   ![image](https://github.com/Vladimir174/monitoring-018/assets/40054398/335bb099-2393-4cc7-aca3-2366f963a06f)

   ![image](https://github.com/Vladimir174/monitoring-018/assets/40054398/b64db917-6aa7-4b0c-8064-f85ef604a02d)

   ![image](https://github.com/Vladimir174/monitoring-018/assets/40054398/37d4b3f2-026f-42c3-b30a-c229a23cd976)

   ![image](https://github.com/Vladimir174/monitoring-018/assets/40054398/0fbe19ea-da41-49c8-b5d2-48e2261e9df8)

6. Настроено оповещение при отсутствии данных от nginx в тг канал. https://t.me/RockMusicDay
   ![image](https://github.com/Vladimir174/monitoring-018/assets/40054398/a1e9f65a-e4d2-486e-b9b1-a9323b4f2606)

   ![image](https://github.com/Vladimir174/monitoring-018/assets/40054398/1bd67488-11b0-4966-8838-789a96e09775)







