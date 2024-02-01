Генерация сетки в метрах
========================

.. figure:: _static/grids-demo.png
   :align: center
   :width: 16cm

   Сгенерированные сетки
   
Инструмент осуществляет генерацию сетки в границах обьектов из векторного слоя. Размер сетки задаётся в метрах. Обьекты могут быть в любом месте земли.

На входе:

*  Мультиполигональный слой с одним или несколькими объектами. Принимается формат Geopackage
*  Шаг сетки в метрах
*  Режим: points (точки), rect (квадраты).
*  Алгоритм обрезки сетки по границам. all (оставлять все квадраты в охвате обьекта), touches (оставлять все квадраты касающиеся обьекта), intersection (обрезать квадраты по границе обьекта).

.. figure:: _static/grid-1000-rect-all.png
   :align: center
   :width: 16cm

   all
   
   
.. figure:: _static/grid-1000-rect-touches.png
   :align: center
   :width: 16cm

   touches
   
   
.. figure:: _static/grid-1000-rect-intersection.png
   :align: center
   :width: 16cm

   intersection
   
   
.. figure:: _static/grid-1000-point-all.png
   :align: center
   :width: 16cm

   all для точек
   
   
.. figure:: _static/grid-1000-point-intersection.png
   :align: center
   :width: 16cm

   touches и intersection для точек

   
.. figure:: _static/grid-planet.png
   :align: center
   :width: 16cm

   Сгенерированные сетки для нескольких полигонов в разных местах глобуса
   

*  выходной формат геоданных - GeoJSON, ESRI Shape, Mapinfo TAB

На выходе:

* Geopackage


Запуск инструмента: https://toolbox.nextgis.com/operation/grid
