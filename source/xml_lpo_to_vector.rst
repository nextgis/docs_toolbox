Конвертация XML: Акт лесопатологического обследования
=====================================================

Конвертация XML-документа Акт лесопатологического обследования.

.. note:: 

   Этот документ обрабатывает только Акт лесопатологического обследования. 
   Если вам нужно сконвертировать документ XML другого типа, воспользуйтесь другими `инструментами конвертации <https://toolbox.nextgis.com/?tags=6>`_:
   
   * `Конвертация данных ЕГРН <https://toolbox.nextgis.com/t/import_egrn?from-related-tools=1>`_ (`поддерживаемые типы документов <https://docs.nextgis.ru/docs_rosreestr_tools/source/rr-import.html#ngq-rr-import-supported>`_), 
   * `Лесная декларация <https://toolbox.nextgis.com/t/xml_decl_to_vector?from-related-tools=1>`_,
   * `Таксационное описание лесосеки <https://toolbox.nextgis.com/t/xml_tol_to_vector?from-related-tools=1>`_,
   * `Проект лесовосстановления <https://toolbox.nextgis.com/t/xml_plv_to_vector?from-related-tools=1>`_,
   * `Выписки ГЛР <https://toolbox.nextgis.com/t/import_glr?from-related-tools=1>`_.

На входе:

* Исходный файл - Единичный файл XML или ZIP с любым количеством XML произвольной вложенности;
* Выходной формат - впишите один из вариантов: ``GPKG, GEOJSON, SHP, TAB``.

На выходе:

* ZIP-архив с файлом в выбранном формате.

Запуск инструмента: https://toolbox.nextgis.com/t/xml_lpo_to_vector

Пример работы инструмента:

.. figure:: _static/xml_lpo_to_vector_result_ru.png
   :name: xml_lpo_to_vector_result_pic
   :align: center
   :width: 20cm

   Пример полученного полигона

**Попробуйте инструмент в действии**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::

   * `Конвертация XML: Таксационное описание лесосеки <https://toolbox.nextgis.com/t/xml_tol_to_vector?from-related-tools=1>`_
   * `Каталог учетных номеров <https://toolbox.nextgis.com/t/plk_catalog?from-related-tools=1>`_
   * `Абрис лесосеки: каталог координат в геоданные <https://toolbox.nextgis.com/t/coords2poly?from-related-tools=1>`_
   * `Подготовка и скачивание данных Sentinel-2 <https://toolbox.nextgis.com/t/download_and_prepare_l8_s2?from-related-tools=1>`_