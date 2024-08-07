# Исследование объявлений о продаже квартир
[Проект](Яндекс.Практикум%20Проект%20№3%20Исследование%20объявлений%20о%20продаже%20квартир.ipynb)  
# Постановка задачи:    
Нужно установить параметры, влияющие на цену объектов сервиса Яндекс.Недвижимость, и научиться определять их рыночную стоимость. 
# Навыки и инструменты:  
* **python**
* **pandas**
* **matplotlib**
# Общий вывод:  
- **Получение данных**:
Мы получили данные безопасным способом при помощи конструкции `try-except` и изучили их при помощи метода `info()`. Затем мы построили гистограммы по всем числовым столбцам.
- **Предобработка данных**:
Полученные данные мы очистили от пропусков и неявных дубликатов. Также мы произвели смену типов там, где это необходимо. Некоторые столбцы мы очистили от аномальных значений.
- **Добавление дополнительных столбцов**: Добавили дополнительные столбцы в таблицу с данными:
 * цена одного квадратного метра
 * день недели публикации объявления
 * месяц публикации объявления
 * год публикации объявления
 * тип этажа квартиры
 * расстояние до центра города в километрах
- **Исследовательский анализ данных**: Изучили следующие параметры объектов:
 * общая площадь
 * жилая площадь
 * площадь кухни
 * цена объекта
 * количество комнат
 * высота потолков
 * этаж квартиры;
 * тип этажа квартиры
 * общее количество этажей в доме;
 * расстояние до центра города в метрах;
 * расстояние до ближайшего аэропорта;
 * расстояние до ближайшего парка;
 * день и месяц публикации объявления.
 
 Мы построили отдельные гистограммы по всем вышеперечисленным параметрам. Также мы изучили как быстро продавались квартиры и какие факторы больше всего влияют на общую (полную) стоимость объекта:
 * Продажа объекта обычно занимает от `45` до `248` дней.
 * Необычно долгими можно считать продажи от `553` дней.
 * Чаще всего продажа занимает около `45.0` дней.
 * `total_area`, `living_area`, `kitchen_area`, `rooms`, `floor_category`, `exposition_year` больше всего влияют на общую полную стоимость. 
 * Можно заметить, что квартиры на первом этаже как правило дешевле, чем квартиры на других этажах.
 * С увеличением количества комнат растёт и цена объекта недвижимости.
 * Цена на объекты недвижимости уменьшается с каждым годом вплоть до 2018 года. Цена - это параметр, на который влияет несколько других факторов. Например, можно заметить, что количество объявлений росло с 2014 по 2018 годы. Это могло повлиять на изменение цены на рынке недвижимости. Также изменение средней общей площади объектов недвижимости могло повлиять на изменение цен.
 
 
 Мы посчитали среднюю цену одного квадратного метра в 10 населённых пунктах с наибольшим числом объявлений и выделили населённые пункты с самой высокой и низкой стоимостью квадратного метра:
 * Населённый пункт с самой высокой стоимостью квадратного метра - Санкт-Петербург
 * Населённый пункт с самой низкой стоимостью квадратного метра - деревня Вахнова Кара
 
 После этого мы описали, как стоимость объектов зависит от расстояния до центра города:
 * Цена объекта недвижимости уменьшается с увеличением расстояния до центра. 
 * Аномальные значения на `27`-ом и `41`-ом киллометрах объясняется малым количеством объектов недвижимости на данных расстояниях (`2` объекта и `1` объект соответственно).
 * На расстоянии `3` киллометра до центра можно заметить большое количество объектов расположены на первом этаже, либо на последнем.
 * На расстоянии `5` киллометров до центра можно большинство объектов расположены между первым и последним этажами.
 
