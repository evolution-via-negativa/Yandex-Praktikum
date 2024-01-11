# Предсказание стоимости жилья
[Проект](Яндекс.Практикум%20Проект%20№10%20Предсказание%20стоимости%20жилья.ipynb)  
# Постановка задачи:    
Нужно обучить модель линейной регрессии на данных о жилье в Калифорнии в 1990 году. На основе данных нужно предсказать медианную стоимость дома в жилом массиве.
# Навыки и инструменты:  
* **python**
* **pyspark**
* **pyspark.ml import.Pipeline**
* **pyspark.ml.tuning.CrossValidator**
* **pyspark.ml.tuning.ParamGridBuilder**
* **pyspark.ml.feature.StringIndexer**
* **pyspark.ml.feature.OneHotEncoder**
* **pyspark.ml.feature.OneHotEncoder**
* **pyspark.ml.feature.VectorAssembler**
* **pyspark.ml.feature.StandardScaler**
* **pyspark.ml.regression.LinearRegression**
* **pyspark.ml.evaluation.RegressionEvaluator**
# Общий вывод:
Результаты работы модели линейной регрессии, обученной на полном наборе данных, чуть лучше, чем результаты работы модели, обученной на неполном наборе данных, по всем трём метрикам. Можно предположить, что существует зависимость между признаком `ocean_proximity` и целевым признаком `median_house_value` и первая модель успешно уловила эту взаимосвязь