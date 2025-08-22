Добавить к фотографиям теги Google Photosphere
==============================================

Случается так, что при записи панорамы к файлу не добавляются нужные тэги, и тогда программа просмотра не понимает, что это сферическая панорама.

Инструмент добавляет к изображениям тэги в соответствии со `спецификацией <https://developers.google.com/streetview/spherical-metadata>`_, сообщающие:

* "это панорама",
* "углы охвата - 360х180"

Соответственно, все изображения должны иметь угол обзора 360x180.

GPano:PoseHeadingDegrees копируется из GPSImgDirection, если такой тэг есть в исходных изображениях.

На входе:

* ZIP-архив с фотографиями. Архив может содержать подпапки.

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

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/panotag/panotag_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/panotag/panotag_outputs_ru.zip>`_ работы инструмента.
