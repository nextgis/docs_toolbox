Таблица Google/Яндекс в Веб ГИС
===============================

Создает и обновляет точечный векторный слой в NextGIS Web на базе таблицы Google Sheets или Яндекс Таблица.

Документ должен быть доступен для чтения по ссылке.

Точки могут быть заданы в таблице двумя способами:

1. Столбцы 'lat' и 'lon'. Система координат - WGS84.
2. Ссылки на объекты на Google-карте. Их можно получить с любого устройства, в том числе мобильного.

На входе:

*  Адрес Веб ГИС, например, https://sandbox.nextgis.com.
*  Логин пользователя Веб ГИС с правами на запись.
*  Пароль пользователя Веб ГИС.
*  ID векторного слоя Веб ГИС для обновления. Оставьте пустым для создания нового слоя.
*  ID ресурса (папки), где будет создан слой. Используйте только в случае создания нового слоя, не обновления имеющегося.
*  URL целиком на таблицу в Google Disk/Яндекс.Диск или идентификатор таблицы в Google Disk (например, '1cKvjCMBZajaortAkdQqVwQ_06LuLm3bHyvybJgmAeQg'). Документ должен быть доступен для чтения по ссылке.
*  Режим: по умолчанию инструмент создаёт новый слой или добавляет данные к имеющемуся (режим ADD). Выберите режим REPLACE, чтобы заменить уже имеющийся слой.

На выходе:

* Созданный/обновленный слой в Веб ГИС

Видео про Яндекс Таблицу

.. raw:: html

   <iframe width="720" height="405" src="https://rutube.ru/play/embed/8c3858379f57e8aeef833c92b290de55/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/QcF7UGVVr5M?si=2MTORwqb0N-0gjb4>`_, `rutube <https://rutube.ru/video/8c3858379f57e8aeef833c92b290de55/?r=wd>`_.

Видео про Google Sheets

.. raw:: html

   <iframe width="720" height="405" src="https://rutube.ru/play/embed/f3a609e3af7f7161144db9388f448340/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/MbZ1ZulLYcU?si=lTyCAoCVRaypqsZv>`__, `rutube <https://rutube.ru/video/f3a609e3af7f7161144db9388f448340/>`__.

Запуск инструмента: https://toolbox.nextgis.com/t/spreadsheet2layer

**Попробуйте инструмент в действии**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::

   * `Таблица в векторный файл <https://toolbox.nextgis.com/t/table2geo?from-related-tools=1>`_