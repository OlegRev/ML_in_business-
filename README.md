## python-flask-docker

Итоговый проект курса "Машинное обучение в бизнесе"

### Стек:
* ML:
    > numpy, pandas, sklearn, xgboost
* API: 
    > flask

### Данные:
* kaggle:
> https://www.kaggle.com/colearninglounge/predicting-pulsar-starintermediate
* UCI(Очищеные данные):
> https://archive.ics.uci.edu/ml/datasets/HTRU2

### Задача:
> На основе непрерывных переменных, описывающих звезды,
> определить действительно ли звезды являются пульсаром или нет.
> 
> Пульсары отличаются своим интегрированным профилем импульса,
который представляет собой периодический пульсирующий сигнал.
Это визуальное представление сигналов излучения пульсара в зависимости от периода его вращения.
>> Вот несколько примеров интегрированных профилей импульсов:
>>* Excess kurtosis of the integrated profile.
>>>(Избыточная резкость пика кривой частотного распределения
интегрированного профиля - резкость пика кривой частотного распределения
измеряет «жирность» хвостов данного распределения.
Положительное превышение резкости пика кривой частотного распределения означает,
что у распределения хвосты больше, чем у нормального распределения.
Это означает, что распределение менее точное и может указывать на больший шум.)
>>* Skewness of the integrated profile.
>>>(Асимметрия интегрированного профиля - измеряет асимметрию распределения.
В этом контексте, если IPP кандидата в звезду имеет отрицательный перекос,
сигнал сначала сильный, но затем быстро спадает.
Если звезда-кандидат имеет положительный перекос,
сигнал сначала будет слабым, а затем достигнет пика в правой части распределения.)
>>* Mean of the integrated profile.
>>>(Среднее значение интегрированного профиля)
>* Бинарная классификация

### Используемые признаки:
* 'Excess kurtosis of the integrated profile'
* 'Skewness of the integrated profile'
* 'Mean of the integrated profile'

### Преобразования признаков:
> StandardScaler

### Модель: 
> XGBClassifier
