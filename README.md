# Optimization-of-model-parameters
Optimization of model parameters for SF

From the [SkillFactory Data Science course] (https://skillfactory.ru/data-scientist).\

## Content
[1. Project description] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Project description)
[2. What case are we solving?] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#What case are we solving?)
[3. Brief information about the data] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Brief information about the data)
[4. Stages of work on the project] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Stages of work on the project)
[5. Results] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Results)
[6. Conclusions:] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Conclusions:)

### Project description
В этом проекте описана работа с датасетом из соревнования Kaggle: Predicting a Biological Response (Прогнозирование биологического ответа). Необходимо предсказать биологический ответ молекул (столбец 'Activity') по их химическому составу (столбцы D1-D1776).

:arrow_up: [к оглавнению] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Content)


### What case are we solving?
Необходимо обучить две модели: логистическую регрессию и случайный лес. Далее нужно сделать подбор гиперпараметров с помощью базовых и продвинутых методов оптимизации. Важно использовать все четыре метода (GridSeachCV, RandomizedSearchCV, Hyperopt, Optuna) хотя бы по разу, максимальное количество итераций не должно превышать 50.

**Quality metric**
В качестве метрики будем использовать F1-score.

## Brief information about the data
Данные представлены в формате CSV.  Каждая строка представляет молекулу. 

    Первый столбец Activity содержит экспериментальные данные, описывающие фактический биологический ответ [0, 1]; 
    Остальные столбцы D1-D1776 представляют собой молекулярные дескрипторы — это вычисляемые свойства, которые могут фиксировать некоторые характеристики молекулы, например размер, форму или состав элементов.


:arrow_up:[к оглавлению] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Content)


### Stages of work on the project
    1. Загружаем данные и анализируем датасет
    2. Используем метод GridSearchCV()
    3. Используем метод RandowizedSearchCV()
    4. Используем библиотеку Huperopt
    5. Используем библиотеку Optuna

:arrow_up:[к оглавлению] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Content)


### Results
Результатом является значение метрики F1-score равное 0,83, полученное с помощью библиотеки Optuna. 

:arrow_up:[к оглавлению] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Content)


### Conclusions:
В ходе данной работы значение метрики F1-score было значительно улучшено по сравнению со стандарстными методами LogisticRegression() и DecisionTreeClassifier().

:arrow_up:[к оглавлению] (https://github.com/littleshadowraven/Optimization-of-model-parameters/blob/main/README.md#Content)