Упрощение полигонов
===================

Инструмент упрощает геометрии полигональных и линейных объектов. Подойдет для упрощения границ административно-территориального деления, растительности и других соприкасающихся друг с другом полигонов. Топология сохраняется, то есть между объектами не появится разрывов и наложений.

На входе:

* Файл линейного или полигонального слоя в OGR-совместимом векторном формате. Для форматов, имеющих несколько файлов указывается ZIP архив с ними.
* Процент упрощения- количество оставляемых вершин. Диапазон от 1 до 100. Для тестирования используйте 90. Чем **выше** процент - тем **больше** упрощение.

На выходе:

* GeoJSON с упрощенной геометрией

.. raw:: html

   <iframe width="720" height="405" src="https://rutube.ru/play/embed/a7a7d0595300bb2efe4af86baf2eb4fd/" frameBorder="0" allow="clipboard-write; autoplay" webkitAllowFullScreen mozallowfullscreen allowFullScreen></iframe>

Посмотреть видео на `youtube <https://youtu.be/X3jrMnyqKQE>`_, `rutube <https://rutube.ru/video/a7a7d0595300bb2efe4af86baf2eb4fd/>`_.

Запуск инструмента: https://toolbox.nextgis.com/t/polysimplifier

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/polysimplifier/polysimplifier_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/polysimplifier/polysimplifier_outputs_ru.zip>`_ работы инструмента.

.. seealso::

   * `Продвинутое упрощение векторных данных <https://toolbox.nextgis.com/t/generalization>`_
   * `Разделить сложные полигоны <https://toolbox.nextgis.com/t/splitcomplex>`_