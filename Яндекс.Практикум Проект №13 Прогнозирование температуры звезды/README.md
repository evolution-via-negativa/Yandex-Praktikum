
# Прогнозирование температуры звезды
[Проект](Яндекс.Практикум%20Проект%20№13%20Прогнозирование%20температуры%20звезды.ipynb)  
# Постановка задачи:    
Необходимо разработать нейронную сеть, которая поможет предсказывать абсолютную температуру на поверхности звезды.
# Навыки и инструменты:  
* **python**
* **numpy**
* **pandas**
* **matplotlib**
* **torch**
* **sklearn**
# Общий вывод:
* в данных присутствуют всего $240$ объектов. Среди них есть звёзды с аномальными значениями абсолютной температуры, которые крайне сложно спрогнозировать
* базовая модель неплохо справилась со своей задачей. На первый взгляд предсказания модели достаточно близки к реальным данным
* лучшая по результатам перебора гиперпараметров модель показала меньшее значение `RMSE`чем `baseline` модель
* тем не менее лучшая модель всё-таки не смогла хорошо спрогнозировать абсолютную температуру для некоторых аномальных значений 
