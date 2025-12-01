Получить историю векторного объекта
===================================

Получить историю изменений объекта из версионируемого векторного слоя NextGIS Web. Подробнее `о версионировании <https://docs.nextgis.ru/docs_ngweb/source/version.html>`_. Включить версионирование можно `в настройках слоя <https://docs.nextgis.ru/docs_ngweb/source/layers.html#create-vector-layer-vers-pic>`_.

На входе:

* Адрес NGW - адрес Веб ГИС, например, https://example.nextgis.com;
* Логин - NextGIS ID или имя пользователя Веб ГИС;
* Пароль пользователя Веб ГИС;
* ID ресурса векторного слоя - Цифры в конце ссылки на ресурс;
* ID объекта в векторном слое, находится в поле ``#``;
* Начальное время - начальная метка времени для получения истории (указывается в формате ГГГГ-мм-дд ЧЧ:ММ:СС, опционально);
* Конечное время - конечная метка времени для получения истории (указывается в формате ГГГГ-мм-дд ЧЧ:ММ:СС, опционально).

На выходе:

* Итоговый GeoPackage. Файл GeoPackage с историей изменения объекта.

Запуск инструмента: https://toolbox.nextgis.com/t/ngw_feature_history

Пример работы инструмента:

.. figure:: _static/ngw_feature_history_result_ru.png
   :name: ngw_feature_history_result_pic
   :align: center
   :width: 14cm

   История изменений точечного объекта

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/ngw_feature_history/ngw_feature_history_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/ngw_feature_history/ngw_feature_history_outputs_ru.zip>`_ работы инструмента.

.. seealso::

   * `Получить отчёт об изменениях ресурса <https://toolbox.nextgis.com/t/ngw_contribution_activity?from-related-tools=1>`_
   * `Структура Веб ГИС в таблицу <https://toolbox.nextgis.com/t/web_gis_structure?from-related-tools=1>`_