# Функция для расчета Retention Rate

## Описание
Необходимо подготовить функцию, которая будет рассчитывать retantion rate пользователей мобильной игры. 
Для расчета на вход подается определенный набор данных, с необходимой информацией.

## Данные 

problem1-reg_data.csv – данные о времени регистрации

- reg_ts - время регистрации
- uid - id пользователя

problem1-auth_data.csv – данные о времени захода пользователей в игру

- reg_ts - время авторизации (входа)
- uid - id пользователя

## Стек

Python (pandas, Numpy, ScyPy, matplotlib, seaborn)

## Ход работы

### Общий анализ данных

Первичный анализ данных на предмет пропущенных значений, особенностей формата данных и т.д.

### Функция

1. Заложить в функцию возможность самостоятельно задавать дату старта и окончания расчета retantion
2. Привести данные о времени регистрации и входа к удобному виду
3. Объединить таблицы с информацией о регистрации и заходах в одну
4. Распределить пользователей на когорты по дням по времени первого входа
5. Рассчитать сколько пользователей из каждой когорты заходили в приложение на n-ный (целевой для расчёта retention) день
6. Рассчитать по этим данным retention
7. Для наглядности добавить визуализацию полученного результата
