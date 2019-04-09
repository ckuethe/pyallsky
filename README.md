# allsky.py

Питон+PHP скрипты для AllSky камеры из Raspberry/Orange Pi + ZWO / QHY / Starlight / .... любой INDI.

Проверено на железе:
* Raspberry Pi 3 + Datyson t7c / t7m (драйвер ZWO ASI 120)
* Raspberry Pi 3 + ZWO ASI 178c
* Orange Pi PC + Starlight Oculus / QHY5 старая шайба чб (через fxload и INDI qhy)
* Tinkerboard / S + QHY5-II

# Возможности

## Сейчас

Сейчас проект может:
* поддерживать разные INDI камеры, найденные через list.py, задаваемые в config.py;
* подбирать выдержку от минимальной до максимальной заданной, стараясь среднее по средней части кадра держать в вилке 55...150 ADU;
* раз в минуту записывать файлы в папку локального веб-сервера, именуя их по дате / времени;
* снабжать кадр timestamp'ом, то есть указанием даты и времени (настраивается);
* поддерживать актуальным файл (симлинк) последнего отснятого кадра;
* удалять старые файлы (выходящие за кол-во дней, указанных в конфиге);
* ежеминутно сохранять данные по выдержке / среднему, данные с датчиков (температура, влажность, давление, ...);
* собирать видеоролик ежесуточно (в 12 дня за сутки от вчерашнего полудня до сейчас)
* веб может показывать:
  * последний отснятый кадр и отображать дату / время его актуальности;
  * любой кадр из архива с возможностью листать кадры с клавиатуры или кликом в вебе;
  * собранные видеоролики;
  * графики с датчиков в разрезе за разное время (час, сутки, неделя, месяц).
* веб может управлять:
  * платой реле / мосфетов / ключей для управления нагрузками.
Подробнее в вики проекта: https://github.com/oleg-milantiev/allsky.py/wiki

## В ближайших планах

Сроки размазаны, но планы чёткие. Описаны на страницах планирования гитхаба https://github.com/oleg-milantiev/allsky.py/milestones 
Участвуй в проекте! Роль найдётся каждому. Можно просто придумывать хотелки и писать их в Issues гитхаба: https://github.com/oleg-milantiev/allsky.py/issues . Но, возможно, твоя роль в чём-то большем?

# Установка

Подробно описана в вики проекта на соответствующей странице: https://github.com/oleg-milantiev/allsky.py/wiki/install
