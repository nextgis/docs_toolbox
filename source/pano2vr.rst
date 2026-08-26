Конвертация панорам Garden Gnome Package в JPEG
===============================================

Извлекает панорамы из пакета Garden Gnome Package (.ggpkg), экспортированного из Pano2VR, и конвертирует их в плоские сферические (equirectangular) JPEG — по одному файлу на каждую точку съёмки тура. Результат — ZIP-архив с панорамами, готовыми к загрузке в NextGIS Web.

На входе:

* Исходный пакет - тур в формате Garden Gnome Package (.ggpkg), экспортированный из Pano2VR.

На выходе:

* ZIP-архив с equirectangular JPEG-панорамами, по одной на каждую точку съёмки.

Панорамы можно прикреплять в качестве вложений к объектам векторного слоя и просматривать на веб-карте, `подробнее <https://docs.nextgis.ru/docs_ngweb/source/feature_edit.html#ngw-attachments-panoramas>`_.

Запуск инструмента: https://toolbox.nextgis.com/t/pano2vr

Пример работы инструмента:

.. todo:: _static/pano2vr_input_ru.png
   :name: pano2vr_input_pic
   :align: center
   :width: 20cm

   Пример исходных данных

.. todo:: _static/pano2vr_result_ru.png
   :name: pano2vr_result_pic
   :align: center
   :width: 20cm

   Пример результата работы инструмента

**Попробуйте инструмент в действии:**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::

   * `Добавление тегов Photospere к фотографиям <https://toolbox.nextgis.com/t/panotag?from-related-tools=1>`_
   * `Фото с EXIF в слой NGW <https://toolbox.nextgis.com/t/exif2resource?from-related-tools=1>`_
   * `Добавление координат к фотографиям <https://toolbox.nextgis.com/t/gpx2exif?from-related-tools=1>`_