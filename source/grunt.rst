Конвертация данных о захоронении грунтов
========================================

Данные из "Реестр районов захоронения грунта, извлеченного при проведении дноуглубительных работ, во внутренних морских водах и в территориальном море Российской Федерации" конвертируются в векторный файл.

На входе:

Таблица XLSX – содержит координаты точек или полигонов захоронений (описываются набором точек) и их атрибуты. Готовые таблицы можно получить на сайте `Росприроднадзора <https://rpn.gov.ru/opendata/7703381225-grunt?sphrase_id=1181168>`_ (необходима авторизация через Госуслуги).

На выходе:

Файл GeoPackage с точками и контурами захоронений в системе координат WGS-84

.. raw:: html

   <iframe width="720" height="405" src="https://rutube.ru/play/embed/147bd4bd5bbe46d41d9c76aa90c31007/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/QUhAjnB86GE?si=ViTBiL7Q2XENw6hu>`_, `rutube <https://rutube.ru/video/147bd4bd5bbe46d41d9c76aa90c31007/>`_.

Запуск инструмента: https://toolbox.nextgis.com/t/grunt

**Попробуйте инструмент в действии**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::

   * `XLSX данных о водных объектах в GeoPackage <https://toolbox.nextgis.com/t/water_usage?from-related-tools=1>`_
   * `Конвертация данных ЕГРН <https://toolbox.nextgis.com/t/import_egrn?from-related-tools=1>`_