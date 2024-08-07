# Определение стоимости автомобилей
[Проект](Яндекс.Практикум%20Проект%20№12%20Определение%20стоимости%20автомобилей.ipynb)  
# Постановка задачи:    
Нужно построить модель для определения стоимости автомобилей.
# Навыки и инструменты:  
* **python**
* **numpy**
* **pandas**
* **matplotlib**
* **sklearn.linear_model.SGDRegressor**
* **lightgbm**
# Общий вывод:
* загрузили данные и провели небольшой разведочный анализ данных
* в данных присутствовали пропуски, дубликаты, аномальные значения и неинформативные признаки, с которыми мы разобрались на этапе предобработки данных
* разделили данные на обучающую и тестовую выборки
* создали модели `SGDRegressor` и `GradientBoosting`
* нашли оптимальные наборы гиперпараметров для обеих моделей при помощи кросс-валидации
* модель `SGDRegressor` обучается чуть быстрее, чем модель `GradientBoosting`
* модель `SGDRegressor` делает предсказания чуть быстрее, чем модель `GradientBoosting`
* модель `GradientBoosting` показала намного меньшее значение `RMSE`, чем модель `SGDRegressor`
* На тестовой выборке результаты совпадают с результатами при кросс-валидации. Следовательно модели удалось уловить зависимость и при этом не переобучиться
* для оптимизации скорости обучения и предсказания рекомендуется использовать модель `SGDRegressor`. Во всех остальных случаях лучше всего подойдёт модель `GradientBoosting`
