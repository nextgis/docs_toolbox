TROPOMI в GeoTIFF
=================

Инструмент конвертирует данные TROPOMI по диоксиду азота в формат GeoTIFF

На входе:

*  Файл данных TROPOMI в формате NetCDF полученный с https://s5phub.copernicus.eu/dhus/#/home. Product type: L2__NO2__, Timeliness: Offline. Пример имени файла: S5P_OFFL_L2__NO2____20190901T091635_20190901T105804_09761_01_010302_20190907T113505.nc


На выходе

*  GeoTIFF готового снимка

Запуск инструмента: https://toolbox.nextgis.com/operation/tropomi2geotiff

Скачать пример исходных данных и результатов расчёта: http://nextgis.ru/data/toolbox/tropomi2geotiff/tropomi2geotiff.zip

Посмотреть пример результата на интерактивной карте: https://demo.nextgis.com/resource/4698/display?panel=layers

.. figure:: _static/tropomi2geotiff.png
   :align: center
   :width: 16cm
   
Исходные сцены должны быть на scihub.copernicus (https://scihub.copernicus.eu), но временно лежат на копии веб-интерфейса Sentinel-5P Pre-Operations Hub: https://s5phub.copernicus.eu/dhus/#/home . Логины от scihub не действуют, нужно использовать s5pguest/s5pguest. 
   
