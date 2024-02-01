Пакетный поиск по кадастровым номерам
=====================================

Инструмент создаёт набор слоёв с границами кадастровых объектов, получая на вход текстовый файл со списком их номеров.
Для работы необходим доступ к `geoservices <https://geoservices.nextgis.com/settings/profile>`_. Авторизация через аккаунт на my.nextgis.com (NextGIS ID)

На входе:

* API-ключ из https://geoservices.nextgis.com/settings/profile (Settings -> Profile).
* Текстовый файл (*.txt) с номерами объектов. Одна строка - один кадастровый номер. Максимально возможное количество номеров - 100.

На выходе:

* Архив с геоданными кадастровых объектов

Запуск инструмента: https://toolbox.nextgis.com/operation/cadnums_to_geodata

Пример исходных данных и результат: https://nextgis.ru/data/toolbox/cadnums_to_geodata/cadnums_to_geodata.zip
