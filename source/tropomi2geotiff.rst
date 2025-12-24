.. todo:: Не работает, убран из tools.rst

TROPOMI в GeoTIFF
=================

Инструмент конвертирует данные TROPOMI по диоксиду азота в формат GeoTIFF

На входе:

*  Файл данных TROPOMI в формате NetCDF, полученный с https://browser.dataspace.copernicus.eu. Product type: L2__NO2__, Timeliness: Offline. Пример имени файла: S5P_OFFL_L2__NO2____20190901T091635_20190901T105804_09761_01_010302_20190907T113505.nc

Такие данные можно скачать на https://browser.dataspace.copernicus.eu или через AWS CLI ``s3://meeo-s5p/OFFL/L2__NO2___/``.


На выходе

*  GeoTIFF готового снимка

Запуск инструмента: https://toolbox.nextgis.com/t/tropomi2geotiff

Посмотреть пример результата на интерактивной карте: https://demo.nextgis.com/resource/4698/display?panel=layers

.. figure:: _static/tropomi2geotiff.png
   :align: center
   :width: 16cm
   
   
**Попробуйте инструмент в действии**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.
