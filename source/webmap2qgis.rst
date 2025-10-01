Веб-карта в проект QGIS
=======================
Инструмент работает с данными Веб ГИС: конвертирует векторный слои и их стили с любой указанной веб-карты в проект QGIS и файл GeoPackage.

На входе:

* Адрес Веб ГИС – ссылка на Веб ГИС на платформе NextGIS, где размещена веб-карта, которую необходимо сконвертировать. Например, ``https://demo.nextgis.com``;
* ID веб-карты - цифры в конце URL веб-карты;
* Логин - NextGIS ID или имя пользователя Веб ГИС, имеющего доступ к веб-карте;
* Пароль – пароль этого пользователя;
* Охват - по умолчанию берётся охват, заданный в настройках карты. При желании можно указать другой. Задаётся в EPSG:4326, формат: низ, лево, верх, право (юг, запад, север, восток). Значения через запятую, разделитель целой и дробной части - точка. Например: ``54.5, 102.5, 59, 116``.

На выходе:

* ZIP-архив с файлом проекта для QGIS (.qgs) и файлом GeoPackage, содержащим векторные слои.

.. raw:: html

   <iframe width="720" height="405" src="https://rutube.ru/play/embed/75b01414079e651694d96f9dc41a1a16/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/ejg4tdYrGdQ>`_, `rutube <https://rutube.ru/video/75b01414079e651694d96f9dc41a1a16/>`_.

Запуск инструмента: https://toolbox.nextgis.com/t/webmap2qgis

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/webmap2qgis/webmap2qgis_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/webmap2qgis/webmap2qgis_outputs_ru.zip>`_ работы инструмента.

.. seealso::

   * `Векторные слои из Веб ГИС в GeoPackage <https://toolbox.nextgis.com/t/ngw_to_gpkg>`_
   * `Структура Веб ГИС в таблицу <https://toolbox.nextgis.com/t/web_gis_structure>`_