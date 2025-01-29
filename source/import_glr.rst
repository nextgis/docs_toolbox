Конвертация выписок ГЛР 
===========================

Инструмент позволяет конвертировать выписки Государственного лесного реестра из формата XML в наборы геоданных.

Поддерживаемые типы выписок:

* выписка на лесной квартал (stateForestRegisterExtractForestQuarter)
* выписка на лесотаксационный выдел (stateForestRegisterExtractForestTaxingAllocation)


На входе:

* Исходный набор данных - Один файл выписки в формате XML

На выходе:

* Файл GPKG в системе координат EPSG:4326

.. figure:: _static/import_glr_result_ru.png
   :name: import_glr_result_pic
   :align: center
   :width: 20cm

   Геоданные, полученные с помощью инструмента, в проекте QGIS

Запуск инструмента: https://toolbox.nextgis.com/t/import_glr

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/import_glr/import_glr_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/import_glr/import_glr_outputs_ru.zip>`_ работы инструмента.
