.. sectionauthor:: Maxim Dubinin <maxim.dubinin@nextgis.com>
.. NextGIS Toolbox TOC

.. _toolbox_intro:

Инструменты
===========

.. _toolbox_dem:

Пакет данных по рельефу
-----------------------



.. figure:: _static/isolines_sample.png
   :align: center
   :width: 16cm
   
   Пример рендринга 
   
Генерация пакета данных по рельефу.

На входе:

* Шаг горизонталей. Целочисленное значение.
* База данных. Выбор из ALOS, GMTED, GEBCO.
* Граница обрезки. Подгрузка заархивированного в zip файла в формате GeoJSON (EPSG:4326).

Результатом работы процесса является набор слоёв:

* Изолинии рельефа с заданным шагом
* Цифровая модель рельефа (разрешение 30 м если территория до 60 гр. с.ш., 250 м если после)
* Свето-теневая отмывка рельефа (разрешение как у ЦМР)

Запуск инструмента: https://toolbox.nextgis.com/operation/dem/exec

Скачать пример результатов: https://demo.nextgis.com/api/resource/4548/export?zipped=true&format=shp

Посмотреть результаты на интерактивной карте: https://demo.nextgis.com/resource/4552/display?panel=layers

.. _toolbox_launch_conditions:


.. _toolbox_split_to_equal:

Разбить на равные части
-----------------------



.. figure:: _static/isolines_sample.png
   :align: center
   :width: 16cm
   
   Разбить на равные части
   
Генерация пакета данных по рельефу.

На входе:

* Слой с полигоном (zip c Shapefile)

Результатом работы процесса является слой:

* Полигоны, с приблизительно одинаковой площадью

Запуск инструмента: https://toolbox.nextgis.com/operation/split_to_equal/exec



Посмотреть результаты на интерактивной карте: https://demo.nextgis.com/resource/4108/display?panel=info


Извлечение высот
----------------

Извлечение значений высот из ЦМР в точках. Возвращает CSV с координатами и высотами.

Запуск инструмента: https://toolbox.nextgis.com/operation/demInPoints/exec

