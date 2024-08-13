.. sectionauthor:: Юлия Григоренко <grigorenko.j@gmail.com>

Конвертация RSC в CSV 
==========================

Конвертация файла классификатора RSC из ГИС Панорама в CSV для анализа. Он используется для сравнения списка условных знаков в Панораме с другими программами.

В ГИС Панорама версии 15 откройте редактор классификатора. Общие данные - Сохранить как. Выберите следующие параметры сохранения:

* Форма отчетов: Краткая. 
* Таблицы: Таблица объектов. 

Полученый файл в формате txt загрузите в инструмент. 

**На входе:** TXT-файл

.. figure:: _static/rsc2csv_input_ru.png
   :name: rsc2csv_input_pic
   :align: center
   :width: 16cm

   Исходный файл TXT

**На выходе:** CSV со списком знаков. 

.. figure:: _static/rsc2csv_output_ru.png
   :name: rsc2csv_output_pic
   :align: center
   :width: 16cm

   Полученный файл CSV

Запуск инструмента: https://toolbox.nextgis.com/operation/rsc2csv

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/rsc2csv/rsc2csv_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/rsc2csv/rsc2csv_outputs_ru.zip>`_ работы инструмента.
