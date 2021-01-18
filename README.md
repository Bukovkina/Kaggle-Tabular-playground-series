# Kaggle Tabular Playground Series - Jan 2021

Здесь представлен python notebook для Kaggle соревнования Tabular Playground Series - Jan 2021. [Kaggle](https://www.kaggle.com/c/tabular-playground-series-jan-2021/overview) Это соревнование направлено на оттачивание своих умений применения регрессионных моделей на табличных данных.

Был проведен первичный анализ данных и применены некоторые регрессионные алгоритмы.

Для данной задачи были использованы следующие модели:

 * Stochastic Gradient Descent (SGD) - Стохастический градиентный спуск [Wiki](https://ru.wikipedia.org/wiki/%D0%A1%D1%82%D0%BE%D1%85%D0%B0%D1%81%D1%82%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D0%B9_%D0%B3%D1%80%D0%B0%D0%B4%D0%B8%D0%B5%D0%BD%D1%82%D0%BD%D1%8B%D0%B9_%D1%81%D0%BF%D1%83%D1%81%D0%BA)
 * Linear Regression - Линейная регрессия [Wiki](https://ru.wikipedia.org/wiki/%D0%9B%D0%B8%D0%BD%D0%B5%D0%B9%D0%BD%D0%B0%D1%8F_%D1%80%D0%B5%D0%B3%D1%80%D0%B5%D1%81%D1%81%D0%B8%D1%8F)
 * Decision Tree - Дерево решений [Wiki](https://ru.wikipedia.org/wiki/%D0%94%D0%B5%D1%80%D0%B5%D0%B2%D0%BE_%D1%80%D0%B5%D1%88%D0%B5%D0%BD%D0%B8%D0%B9)
 * Random Forest - Случайный лес [Wiki](https://ru.wikipedia.org/wiki/Random_forest)
 * K-Nearest Neighbors (k-NN) - Метод k-ближайших соседей [Wiki](https://ru.wikipedia.org/wiki/%D0%9C%D0%B5%D1%82%D0%BE%D0%B4_k-%D0%B1%D0%BB%D0%B8%D0%B6%D0%B0%D0%B9%D1%88%D0%B8%D1%85_%D1%81%D0%BE%D1%81%D0%B5%D0%B4%D0%B5%D0%B9)
 * CatBoost [Wiki](https://ru.wikipedia.org/wiki/CatBoost)
 * XGBoost [Wiki](https://en.wikipedia.org/wiki/XGBoost)
 * Neural Network - Нейронная сеть [Wiki](https://ru.wikipedia.org/wiki/%D0%9D%D0%B5%D0%B9%D1%80%D0%BE%D0%BD%D0%BD%D0%B0%D1%8F_%D1%81%D0%B5%D1%82%D1%8C)


Оценка результатов алгоритмов производится по среднеквадратичной ошибке [Wiki](https://en.wikipedia.org/wiki/Root-mean-square_deviation):
	
	RMSE = sqrt(1/n * sum((y - y_pred)^2))


## Результаты

Ниже представлены значения среднеквадратичной ошибки на тестовых данных, посчитанной после отправки результатов предсказаний на страницу соревнования Kaggle. 

| Регрессионная модель |    RMSE    |
|:--------------------:|:----------:|
| SGD Regressor| 0.72779 |
| Linear Regression | 0.72782 |
| Decision Tree Regressor | 0.72041 |
| Random Forest Regressor | 0.71321 |
| k-Neighbors Regressor | 0.76278 |
| CatBoost Regressor | 0.70452 |
| CatBoost Regressor + K-Fold| 0.69966 |
| XGBoost Regressor | 0.70123 |
| XGBoost Regressor + K-Fold| 0.70086 |
| Neural Network | 0.71344 |
| Avg of all predictions | 0.70961 |



 