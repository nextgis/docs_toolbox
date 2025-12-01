Таблица в векторный файл
========================

Конвертация файла электронной таблицы в векторный файл в выбранном формате.

На входе:

*  Электронная таблица в одном из форматов: ODS, XLSX, CSV. Широта и долгота должны располагаться в отдельных колонках и называться соответственно ``lat`` и ``lon``. Система координат - WGS84, формат записи - градусы с десятичными долями.
*  Опционально: формат выходного файла. Укажите один из списка:


    - ESRI Shapefile
    - GeoPackage
    - GeoJSON
    - TAB
    - MIF
    - SQL
    - CSV
    

*  Опционально: список типов полей для выходного векторного файла, которые соответствуют колонкам в исходной таблице. Необходимо указать через запятую без кавычек. Возможные варианты: ``Integer`` (целое число), ``Real`` (вещественное число), ``String`` (текст), ``Date`` (YYYY-MM-DD) (дата в формате гггг-мм-дд), ``Time`` (HH:MM:SS) (время в формате чч:мм:сс) , ``DateTime`` (YYYY-MM-DD HH:MM:SS) (дата и время в формате гггг-мм-дд чч:мм:сс). Пример: ``Integer,Real,Real,String,String,String``.

На выходе:

* ZIP-архив с векторным файлом. Этот архив вы можете, не распаковывая, импортировать в NextGIS QGIS или NextGIS Web.

Запуск инструмента: https://toolbox.nextgis.com/t/table2geo

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/table2geo/table2geo_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/table2geo/table2geo_outputs_ru.zip>`_ работы инструмента.

.. seealso::

   * `Таблица Google/Яндекс в Веб ГИС <https://toolbox.nextgis.com/t/spreadsheet2layer?from-related-tools=1>`_
   * `Каталог координат в геоданные <https://toolbox.nextgis.com/t/coords2poly?from-related-tools=1>`_
   * `Абрис лесосеки: экспликация (промеры) в геоданные <https://toolbox.nextgis.com/t/explication2poly?from-related-tools=1>`_
   * `Объединение слоя и таблицы по полю <https://toolbox.nextgis.com/t/join_by_field?from-related-tools=1>`_