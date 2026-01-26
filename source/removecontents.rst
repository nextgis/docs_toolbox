Удалить содержимое слоёв
========================
Инструмент удаляет все объекты в векторных слоях указанной группы Веб ГИС на платформе NextGIS. Сами слои остаются.

NextGIS Web (NGW) — это система управления геоданными. Вы можете бесплатно получить к ней доступ после `регистрации <https://docs.nextgis.ru/docs_ngcom/source/create.html>`_. В системе можно хранить геоданные, создавать интерактивные карты, открывать к ним доступ для коллег и клиентов, редактировать данные прямо на карте и в таблицах, а также обрабатывать их с помощью специализированных инструментов Toolbox. `Подробнее о возможностях <https://docs.nextgis.ru/docs_ngweb/source/general.html>`_.

На входе:

* Адрес Веб ГИС – ссылка (URL) на Веб ГИС, например, https://demo.nextgis.com.
* Логин - имя пользователя Веб ГИС.
* Пароль – пароль пользователя Веб ГИС.
* ID группы - числовое значение, ID ресурса группы в Веб ГИС, в слоях которой нужно удалить все объекты.

На выходе:

* Текстовое сообщение о том, что содержимое слоёв удалено.

.. raw:: html

   <iframe width="720" height="405" src="https://rutube.ru/play/embed/1db7663baf849b62d4446cbc60da968a/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/W-GtFRjQx2M>`_, `rutube <https://rutube.ru/video/1db7663baf849b62d4446cbc60da968a/>`_.

Запуск инструмента: https://toolbox.nextgis.com/t/removecontents

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/removecontents/removecontents_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

.. seealso::

   * `Объединение двух векторных слоёв Веб ГИС <https://toolbox.nextgis.com/t/ngw_merge_layers?from-related-tools=1>`_
   * `Дублировать векторный слой nextgis.com <https://toolbox.nextgis.com/t/ngw_copy_layer?from-related-tools=1>`_
   * `Векторные слои из архива в Веб ГИС <https://toolbox.nextgis.com/t/layers2ngw?from-related-tools=1>`_
