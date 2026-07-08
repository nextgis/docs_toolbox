Скачивание Landsat Analysis Ready Data (GLAD ARD)
================================================

Генерирует команды для удобного скачивания Landsat Analysis Ready Data (GLAD ARD) с https://glad.umd.edu/ard/home. 

Данные организованы следующим образом:

ARD-ID тайла формируется из координат нижнего левого угла ячейки сетки. Вы можете посмотреть `разграфку тайлов <https://demo-ru.nextgis.com/resource/10150/display?panel=layers>`_ на онлайн-карте.

.. figure:: _static/download_glad_tile_id_ru.png
   :name: download_glad_input_pic
   :align: center
   :width: 20cm

   Разграфка тайлов ARD, выбран тайл 006E_46N

Нумерация 16-дневных интервалов сквозная с 1997 года. Идентификаторы интервалов интересующего вас периода можно посмотреть в :download:`таблице <https://glad.umd.edu/users/Potapov/ARD/16d_intervals.xlsx>`.

На входе:

* CSV файл со списком ID тайлов, записанных в соответствующем формате, например ``039E_44N``;
* Начальный интервал - цифровой ID первого 16-дневного интервала, с которым пересекается интересующий вас период;
* Конечный интервал - цифровой ID последнего 16-дневного интервала нужного периода.

На выходе:

* BAT-файл для Windows для скачивания через стандартный Powershell. Не требует никак дополнительных установок;
* BAT-файл для Windows для скачивания через AWS. Требует предварительной установки AWS CLI https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html;
* TXT-файл со списком адресов для утилит закачек, например wget или curl.

Запуск инструмента: https://toolbox.nextgis.com/t/download_glad

Пример данных, скачанных с помощью полученного BAT-файла:


.. figure:: _static/download_glad_result_ru.png
   :name: download_glad_result_pic
   :align: center
   :width: 20cm

   Тайлы в NextGIS QGIS, открытые поверх разграфки

**Попробуйте инструмент в действии**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::  

   * `Cцены Sentinel-2 в GPKG <https://toolbox.nextgis.com/t/s2_search?from-related-tools=1>`_
   * `Подготовка и скачивание данных Sentinel-2 <https://toolbox.nextgis.com/t/download_and_prepare_l8_s2?from-related-tools=1>`_
   * `Радиометрическая калибровка данных Landsat <https://toolbox.nextgis.com/t/landsat_to_radiance?from-related-tools=1>`_
   * `Расчёт спектрального альбедо объектов по данным Landsat <https://toolbox.nextgis.com/t/landsat_to_reflectance?from-related-tools=1>`_
