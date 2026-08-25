Выгрузка образов из NextGIS Container Registry
==============================================

Выгрузка образов Docker из NextGIS Container Registry в архив \*.tar.gz. Это помогает производить установку и обновление ПО в отсутствие выхода в интернет.

Для запуска инструмента выгрузки можно использовать любой аккаунт NextGIS ID, в том числе на бесплатном плане, однако при запуске инструмента потребуется указать ваш логин и пароль для доступа к NextGIS Container Registry, полученный при поставке продукта.

.. admonition:: Инструкции по установке и обновлению серверного ПО NextGIS

   * `NextGIS Web <https://docs.nextgis.ru/docs_ngweb/source/ngw_op.html>`_
   * `GeoServices <https://docs.nextgis.ru/docs_geoserv_prem/source/index.html>`_
   * `NextGIS Toolbox <https://docs.nextgis.ru/docs_toolbox_prem/source/index.html>`_

На входе:

* Дистрибутив. Выберите один из вариантов:

  - NextGIS Web Standard
  - NextGIS Web Standard + Whitelabel
  - NextGIS Web Extended
  - NextGIS Web Extended + Whitelabel
  - NextGIS GeoServices
  - NextGIS Toolbox
  - Nominatim
  - BusyBox (test)

* Версия. Укажите версию продукта для экспорта Docker-образов.
* Логин и пароль для доступа к NextGIS Container Registry. Предоставляется службой поддержки NextGIS при поставке продукта.

На выходе:

* \*.tar.gz архив. Образы можно импортировать в Docker с помощью команды ``docker load -i <archive_name>.tar.gz``.

Запуск инструмента: https://toolbox.nextgis.com/t/ngcr_export

Пример работы инструмента:

.. todo:: _static/ngcr_export_input_ru.png
   :name: ngcr_export_input_pic
   :align: center
   :width: 20cm

   Пример исходных данных

.. todo:: _static/ngcr_export_result_ru.png
   :name: ngcr_export_result_pic
   :align: center
   :width: 20cm

   Пример результата работы инструмента

**Попробуйте инструмент в действии:**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

