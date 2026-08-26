Добавление тегов Photospere к фотографиям
==============================================

Случается так, что при записи панорамы к файлу не добавляются нужные тэги, и тогда программа просмотра не понимает, что это сферическая панорама.

Инструмент добавляет к изображениям тэги в соответствии со `спецификацией <https://developers.google.com/streetview/spherical-metadata>`_, сообщающие:

* "это панорама",
* "углы охвата - 360х180"

Соответственно, все изображения должны иметь угол обзора 360x180.

GPano:PoseHeadingDegrees копируется из GPSImgDirection, если такой тэг есть в исходных изображениях.

На входе:

* ZIP-архив с фотографиями или одиночный файл JPG. Архив может содержать подпапки.

На выходе:

* ZIP-архив с фотографиями, к которым добавлены теги. Все изображения будут лежать в корне архива.

Такую панораму можно `прикрепить к векторному объекту на веб-карте <https://docs.nextgis.ru/docs_ngweb/source/feature_edit.html#ngw-attachments>`_ в NextGIS Web.

Запуск инструмента: https://toolbox.nextgis.com/t/panotag

Пример работы инструмента:

.. figure:: _static/panotag_input.png
   :name: panotag_input_pic
   :align: center
   :width: 20cm

   Пример исходного изображения без нужных тэгов

.. figure:: _static/panotag_result.png
   :name: panotag_result_pic
   :align: center
   :width: 20cm

   Просмотр того же изображения как сферической панорамы

**Попробуйте инструмент в действии**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::

   * `Добавление координат к фотографиям <https://toolbox.nextgis.com/t/gpx2exif?from-related-tools=1>`_
   * `Фото с EXIF в слой NGW <https://toolbox.nextgis.com/t/exif2resource?from-related-tools=1>`_
   * `Конвертация панорам Garden Gnome Package в JPEG <https://toolbox.nextgis.com/t/pano2vr?from-related-tools=1>`_
