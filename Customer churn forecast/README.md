# Customer Churn Prediction for TeleDom

## Project Overview

TeleDom, a telecommunications operator, aims to reduce customer churn by identifying users who are likely to terminate their contracts. To do this, TeleDom's team has collected customer data including personal information, contract details, and subscribed services. The goal of this project is to build a machine learning model that can predict customer churn based on this data.

## Data Description

The project uses the following datasets:

- `contract_new.csv`: Contract information (start/end dates, payment type, monthly/total charges, etc.)
- `personal_new.csv`: Personal data (gender, senior citizen status, marital status, dependents)
- `internet_new.csv`: Internet service details (connection type, security options, backup, streaming, etc.)
- `phone_new.csv`: Phone service information (multiple lines)

All datasets are linked by a common key: `customerID`.

## Project Plan

1. **Data Loading**  
   Load and inspect the datasets.

2. **Exploratory Data Analysis (EDA) & Preprocessing**  
   Analyze each dataset individually, handle missing values and anomalies, and prepare for merging.

3. **Merging Data**  
   Combine all relevant features into a single DataFrame using `customerID`.

4. **Merged Data Analysis & Feature Engineering**  
   Analyze distributions and correlations. Create or transform features if necessary.

5. **Data Preparation**  
   Encode categorical variables and scale numerical features. Split data into training and test sets.

6. **Model Training**  
   Train at least two machine learning models. Perform hyperparameter tuning for at least one model.

7. **Model Evaluation**  
   Select the best model and evaluate it on the test set.

8. **Conclusion and Business Recommendations**  
   Summarize findings, present model performance, and provide actionable recommendations for reducing churn.

---

_# Прогноз оттока клиентов для компании «ТелеДом»_

## Обзор проекта

Оператор связи «ТелеДом» стремится снизить отток клиентов, определяя тех, кто может разорвать договор. Для этого собраны данные о клиентах, включая личную информацию, детали договоров и подключённые услуги. Цель проекта — построить модель машинного обучения для предсказания оттока клиентов.

## Описание данных

В проекте используются следующие наборы данных:

- `contract_new.csv`: Информация о договоре (даты, тип оплаты, расходы и т.д.)
- `personal_new.csv`: Персональные данные (пол, пенсионный статус, наличие супруга/детей)
- `internet_new.csv`: Информация об интернет-услугах (тип подключения, безопасность, стриминг и т.д.)
- `phone_new.csv`: Информация об услугах телефонии (несколько линий)

Все данные связаны через идентификатор `customerID`.

## План проекта

1. **Загрузка данных**  
   Загрузка и первичный осмотр датасетов.

2. **Анализ и предобработка данных**  
   Изучение каждого набора данных, обработка пропусков и аномалий.

3. **Объединение данных**  
   Объединение всех признаков в один датафрейм по `customerID`.

4. **Анализ объединённого датафрейма и генерация признаков**  
   Анализ распределений и корреляций. При необходимости — создание новых признаков.

5. **Подготовка данных**  
   Кодирование категориальных и масштабирование числовых признаков. Деление на обучающую и тестовую выборки.

6. **Обучение моделей**  
   Обучение как минимум двух моделей, подбор гиперпараметров хотя бы для одной из них.

7. **Оценка моделей**  
   Выбор лучшей модели и проверка её качества на тестовой выборке.

8. **Вывод и рекомендации**  
   Подведение итогов, демонстрация результатов модели и рекомендации для бизнеса по снижению оттока клиентов.
