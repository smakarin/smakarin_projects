
## Анализ возможной прибыли и рисков добычи нефти в регионе
### Набор инструментов
Отработка техники boostrap;   
Работа с метриками бизнеса: валовая, операционная, чистая прибыль, конверсии, онлайн и офлайн показатели;  
Визуализация seaborn.
### Вводные данные
Данный проект выполняется для добывающей компании, которой нужно решить, где бурить новую скважину.
Предоставлены данные о пробах нефти в трёх регионах: в каждом 10 000 месторождений, где измерили качество нефти и объём её запасов.
Необходимо построить модель машинного обучения, которая поможет определить регион, где добыча принесёт наибольшую прибыль.
### Цель

Выбрать регион с максимальной прибылью от добычи нефти и минимальным риском ошибки.

### Структура проекта

1. Загрузка и подготовка данных.
2. Обучим и проверка на валидационной выборке модели для каждого региона. Используем метрику RMSE.
3. Создание фукции для расчета прибыли.
4. Примеение Bootstrap для расчета рисков и прибыли для каждого региона.
5. Выбор регион дляи разработки месторождений. 

### Общий вывод  

В данном проекте был проведен анализ нефтяных месторождений в трех регионах с целью выбора наиболее перспективного.
Для этого были произведены следующие действия:

* Произведена первичная обработка данных;
* Произведен первичный анализ каждого региона, изучены корреляции признаков с целевым, изучены распределения целевого признака.
    * Регионы 0 и 2 схожи друг с другом - имеют нормальное распределение объемов месторождений и схожии корреляции признаков.
    * Регион 1 имеет 100% корреляцию одного признака с целевым. Распределение объемов не нормальное;
* Обучены модели линейной регрессии и произведены предсказания объема месторождений каждого региона.
    * Наилучший результат прогнозирования получен в Регионе 1 - среднеквадратичное отклонение меньше 1 тыс баррелей.
    * В Регионах 0 и 2 отклонение равно 37 и 40 тыс. баррелей, но средние значения всей выборки спрогнозированы точно;
* Найден минимальный средний объем месторождений в регионе, при котором добыча нефти будет безубыточной - 11 111 барелей;
* Построена функция расчета прибыли по набору отобранных месторождений и предсказаний модели. Для выборки из топ-200 самых объемных (согласно прогнозы модели) месторождений наиболее прибыльным является Регион 2;
* Применена техника Bootstrap с 1000 выборок для нахождения средней прибыли, 95% доверительного интервала и риска убытков.
    * Риска получения убытков при текущем уровне цен нет ни в одном из регионов.
    * По средним значениям прибыли и доверитльному интервалу наиболее прибыльным регионом является Регион_1.