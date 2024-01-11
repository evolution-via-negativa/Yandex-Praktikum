# Обучение с учителем

[Проект](./Яндекс.Практикум%20«Обучение%20с%20учителем»%20на%20GitHub/Яндекс.Практикум%20«Обучение%20с%20учителем»%20на%20GitHub.ipynb)

# Постановка задачи:  
	* Нужно спрогнозировать, уйдёт клиент из банка в ближайшее время или нет по предоставленным историческим данным о поведении клиентов и расторжении договоров с банком, а также построить модель с предельно большим значением F1-меры.
# Навыки и нструменты:  
	* python  
	* pandas
	* matplotlib
	* sklearn.dummy.DummyClassifier
	* sklearn.tree.DecisionTreeClassifier 
	* sklearn.ensemble.RandomForestClassifier 
	* sklearn.linear_model.LogisticRegression
# Вывод:  
	* Наилучшее значение F1-меры для модели DecisionTreeClassifier с техникой upsampling — 0.5748  
	* Наилучшее значение F1-меры для модели RandomForestClassifier с техникой upsampling — 0.6403  
	* Наилучшее значение F1-меры для модели LogisticRegression с техникой upsampling — 0.4527  
	* Оптимальное значение параметра max_depth для модели DecisionTreeClassifier с техникой upsampling — 6  
	* Оптимальные значения параметров max_depth и n_estimators для модели RandomForestClassifier с техникой upsampling — 10 80  
	* Оптимальное значение параметра max_iter для модели LogisticRegression с техникой upsampling — 200  
	* Значение F1-меры на тестовой выборке для наилучшей модели RandomForestClassifier — 0.622  
