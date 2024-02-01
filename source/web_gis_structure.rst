Структура Веб ГИС в таблицу
===========================

Создаёт электронную таблицу формата .xlsx со структурой Веб ГИС (списком ресурсов).

На входе:

* Адрес Веб ГИС - полный адрес Веб ГИС, например, https://sandbox.nextgis.com
* Логин – имя пользователя Веб ГИС
* Пароль – пароль пользователя Веб ГИС
* Тип ресурса – необходимо указать тип ресурса, по которому будет произведен фильтр среди всех ресурсов данной Веб ГИС. Возможные варианты:
all – все ресурсы Веб ГИС

resource_group – группа ресурсов (директория)

postgis_layer – слой PostGIS

wmsserver_service – сервис WMS

baselayers – базовая карта, подложка

postgis_connection – соединение PostGIS

webmap – веб-карта

wfsserver_service – сервис WFS

vector_layer – векторный слой

raster_layer – растровый слой

mapserver_style – стиль MapServer

qgis_vector_style – векторный стиль QGIS

raster_style – растровый стиль

file_bucket

lookup_table - справочник

wmsclient_layer – слой WMS

wmsclient_connection – соединение WMS

formbuilder_form - форма

trackers_group – группа трекеров

tracker - трекер

collector_project – проект Collector

На выходе:

* Таблица XLSX с перечнем найденных в Веб ГИС ресурсов.

Запуск инструмента: https://toolbox.nextgis.com/operation/web_gis_structure
