.. sectionauthor:: Maxim Dubinin <maxim.dubinin@nextgis.com>
.. NextGIS Toolbox TOC

.. _toolbox_intro:

Инструменты
===========

.. _toolbox_dem:

Пакет данных по рельефу
-----------------------

Генерация пакета данных по рельефу.

Результатом работы процесса является набор слоёв:

* Изолинии рельефа с заданным шагом
* Цифровая модель рельефа (разрешение 30 м если территория до 60 гр. с.ш., 250 м если после)
* Свето-теневая отмывка рельефа (разрешение как у ЦМР)

Запуск инструмента: https://toolbox.nextgis.com/operation/dem/exec

Скачать пример результатов: http://nextgis.ru/data/examples/dem_all.zip

Посмотреть результаты на интерактивной карте: https://demo.nextgis.com/resource/4108/display?panel=info

.. _toolbox_launch_conditions:


Извлечение высот
----------------

Извлечение значений высот из ЦМР в точках. Возвращает CSV с координатами и высотами.

Запуск инструмента: https://toolbox.nextgis.com/operation/demInPoints/exec

