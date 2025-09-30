Геокодировать таблицу
=====================

Инструмент распознает адреса в поданном на вход файле CSV и добавляет в файл информацию об их координатах. Необходимо иметь лицензию на использование соответствующего геокодера.

На входе:

*  Исходные данные - файл CSV с перечнем адресов. Первая строка должна содержать названия полей (столбцов). Кодировка файла - UTF-8.
*  Поле с адресом - имя поля (столбца) в исходном файле CSV, где содержится информация об адресах.
*  Геокодер - выберите один из вариантов: Nominatim, Google или Yandex. Для использования Google и Yandex нужно иметь соответствующий ключ.
*  API ключ - ключ для запуска выбранного геокодера. Для Nominatim оставьте пустым.


.. note::
    **Как получить API ключ для геокодера**

    Яндекс.Геокодер -  https://developer.tech.yandex.ru/services/ (при создании выберите API ключ **JavaScript API и HTTP Геокодер**)

    Geocoding API от Google - https://developers.google.com/maps/documentation/geocoding/usage-and-billing



На выходе:

*  Файл CSV, помимо исходной информации содержащий два дополнительных столбца с координатами (широта и долгота).

Запуск инструмента: https://toolbox.nextgis.com/t/geocodetable

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/geocodetable/geocodetable_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/geocodetable/geocodetable_outputs_ru.zip>`_ работы инструмента.

.. seealso::

    * `Таблица в векторный файл <https://toolbox.nextgis.com/t/table2geo>`_
    * `Таблица Google/Яндекс в Веб ГИС <https://toolbox.nextgis.com/t/spreadsheet2layer>`_
    * `Парсер адреса из CSV <https://toolbox.nextgis.com/t/postal>`_
    * `Генерирует карту в Веб ГИС по таблице со списком кодов регионов ОКАТО и вашим числовым значениям <https://toolbox.nextgis.com/t/infomap>`_