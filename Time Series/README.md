# Taxi Order Prediction

## Project Description

This project aims to solve the problem of predicting the number of taxi orders for the next hour at airports for the company **"Chyotnoye Taxi"**. The goal is to build a model based on historical taxi order data that can accurately predict the number of orders for the upcoming hour. This will help the company efficiently manage the number of drivers during peak hours.

The metric for evaluating the model's performance is **RMSE** (Root Mean Squared Error). The target is to achieve an RMSE value on the test set of no more than **48**.

## Data Description

Taxi order data is stored in the file `taxi.csv`. The main columns in the data are:

- `timestamp` — the timestamp of the order (in date and time format).
- `num_orders` — the number of taxi orders at that specific time.

The data contains information about orders at airports, which needs to be processed for further analysis and model training.

## Project Instructions

1. **Data Loading**: Load the data from the `taxi.csv` file, located in the `/datasets/` directory.

2. **Resampling**: Resample the data to hourly intervals for analysis (resampling by one hour).

3. **Data Analysis**: Perform a time series analysis to identify trends, seasonality, and other patterns.

4. **Model Training**:
   - Split the data into training and test sets (10% of the data should be the test set).
   - Train various machine learning models with different hyperparameters.

5. **Model Evaluation**: Evaluate the model on the test set and measure the RMSE metric.

6. **Conclusion**: Make conclusions based on the model's results and suggest potential improvements.

---

# Прогнозирование заказов такси

## Описание проекта

Проект нацелен на решение задачи прогнозирования количества заказов такси на следующий час в аэропортах для компании **«Чётенькое такси»**. Задача состоит в том, чтобы на основе исторических данных о заказах такси построить модель, которая сможет точно предсказать число заказов на следующий час. Это поможет компании эффективно управлять количеством водителей в периоды пиковой нагрузки.

Метрика для оценки качества модели — **RMSE** (Root Mean Squared Error). Цель — добиться значения RMSE на тестовой выборке не более **48**.

## Описание данных

Данные о заказах такси содержатся в файле `taxi.csv`. Основные столбцы данных:

- `timestamp` — временная метка заказа (в формате даты и времени).
- `num_orders` — количество заказов такси в данный момент времени.

Данные содержат информацию о заказах в аэропортах, которые нужно обработать для дальнейшего анализа и обучения модели.

## Инструкция по выполнению

1. **Загрузка данных**: Необходимо загрузить данные из файла `taxi.csv`, который находится в каталоге `/datasets/`.
   
2. **Ресемплирование**: Привести данные к часовому интервалу для анализа (ресемплирование по одному часу).

3. **Анализ данных**: Провести анализ временных рядов, выявить тренды, сезонность и другие закономерности.

4. **Обучение модели**:
   - Разделите данные на обучающую и тестовую выборки (10% данных — тестовая выборка).
   - Обучите различные модели машинного обучения с разными гиперпараметрами.
   
5. **Оценка модели**: Проверьте модель на тестовой выборке и измерьте метрику RMSE.

6. **Выводы**: Сделайте выводы по результатам работы модели и предложите возможные улучшения.
