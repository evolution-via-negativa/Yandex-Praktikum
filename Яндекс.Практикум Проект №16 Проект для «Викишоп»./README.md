# Проект для «Викишоп»
[Проект](Яндекс.Практикум%20Проект%20№16%20Проект%20для%20«Викишоп».ipynb)  
# Постановка задачи:
Обучить модель классифицировать комментарии на позитивные и негативные.
# Навыки и инструменты:  
* **python**
* **numpy**
* **pandas**
* **matplotlib**
* **optuna**
* **nltk**
* **spacy**
* **sklearn.dummy.DummyClassifier**
* **sklearn.linear_model.LogisticRegression**
* **sklearn.tree.DecisionTreeClassifier**
* **sklearn.ensemble.RandomForestClassifier**
# Общий вывод:
* в данных присутствует явно выраженный дисбаланс классов
* в данных отсутствуют пропущенные значения
* в данных отсутствуют дубликаты
* `LogisticRegression` ожидаемо справилась с прогнозированием токсичности лучше, чем `DummyClassifier`
* `LogisticRegression` справилась с прогнозированием токсичности лучше, чем более сложные модели - `DecisionTreeClassifier`, `RandomForestClassifier`
* Значение `F1 score` больше порогового значения $0.75$ на тестовой выборке
