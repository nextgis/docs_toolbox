Обрезать PBF по прямоугольнику
==============================

Инструмент выкачивает OSM PBF из сети и обрезает его по границе Bounding Box (bbox). Строку границы можно сгенерировать на сайте https://boundingbox.klokantech.com.

На входе:

* Адрес файла PBF. URL файла pbf. Пример:  https://nextgis.com/data/toolbox_static_testfiles/osmclip_bbox/maldives-latest.osm.pbf
* BBOX. Охват в формате CSV, пример: 72.961503,3.748809,72.978497,3.76609.

На выходе:

* Обрезанный PBF

Запуск инструмента: https://toolbox.nextgis.com/operation/osmclip_bbox

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/osmclip_bbox/osmclip_bbox_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/osmclip_bbox/osmclip_bbox_outputs_ru.zip>`_ работы инструмента.
