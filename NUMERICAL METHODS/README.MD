# Car Price Prediction

## Project Overview
The used car sales service "Not Crashed, Not Painted" is developing an application to attract new customers. This app will allow users to estimate the market value of their car. 

Your task is to build a model capable of predicting car prices based on technical characteristics, equipment, and prices of other cars.

## Key Requirements
The customer values the following criteria:
- **Prediction quality** (Root Mean Squared Error, RMSE should be less than 2500)
- **Model training time**
- **Model inference time**

## Instructions
To strengthen the research, do not limit yourself to gradient boosting models. Sometimes simpler models perform better. These rare cases are easy to miss if you only apply boosting.

### Steps to Complete:
1. **Load the data** from `/datasets/autos.csv`.
2. **Explore the data**, fill in missing values, and handle anomalies. Remove uninformative features if necessary.
3. **Prepare datasets** for training the models.
4. **Train multiple models**, including at least one LightGBM and one non-boosting model. Tune different hyperparameters.
5. **Analyze training time, inference time, and model quality**.
6. **Select the best model** based on customer criteria and evaluate its performance on the test set.

### Notes:
- Use **RMSE** as the evaluation metric.
- **Learn and apply LightGBM** for gradient boosting.
- Measure execution time for model training and inference.
- Gradient boosting models can take a long time to train, so modify only **2-3 parameters**.
- If Jupyter Notebook becomes slow, delete unnecessary variables using:
  ```python
  del features_train
  ```

## Dataset Description
The dataset is stored in `/datasets/autos.csv`. It contains the following features:

| Feature | Description |
|---------|-------------|
| `DateCrawled` | Date the ad was scraped from the database |
| `VehicleType` | Type of car body |
| `RegistrationYear` | Year the car was registered |
| `Gearbox` | Transmission type |
| `Power` | Engine power (HP) |
| `Model` | Car model |
| `Kilometer` | Mileage (km) |
| `RegistrationMonth` | Month the car was registered |
| `FuelType` | Type of fuel used |
| `Brand` | Car brand |
| `Repaired` | Whether the car was repaired or not |
| `DateCreated` | Date the ad was created |
| `NumberOfPictures` | Number of car pictures |
| `PostalCode` | Owner's postal code |
| `LastSeen` | Date of last user activity |

### Target Variable:
- `Price` — Car price (in euros)

## Evaluation Criteria
Reviewers will check:
- Whether all required steps were completed
- How the data was preprocessed
- Which models and hyperparameters were considered
- Whether code duplication was avoided
- The quality of conclusions drawn
- Code structure and readability
- Code cleanliness and organization

---

# Определение стоимости автомобилей

## Описание проекта
Сервис продажи автомобилей с пробегом "Не бит, не крашен" разрабатывает приложение для привлечения новых клиентов. В нём пользователи смогут узнать рыночную стоимость своего автомобиля.

Ваша задача — построить модель, которая сможет предсказывать цены автомобилей на основе их технических характеристик, комплектации и цен других автомобилей.

## Ключевые требования
Заказчик оценивает проект по следующим критериям:
- **Качество предсказания** (метрика RMSE должна быть меньше 2500)
- **Время обучения модели**
- **Время предсказания модели**

## Инструкция по выполнению
Для более полного исследования попробуйте не только градиентный бустинг. Иногда простые модели работают лучше. Такие редкие случаи легко упустить, если использовать только бустинг.

### Основные шаги:
1. **Загрузите данные** из `/datasets/autos.csv`.
2. **Изучите данные**, заполните пропущенные значения и обработайте аномалии. Удалите неинформативные признаки, если необходимо.
3. **Подготовьте выборки** для обучения моделей.
4. **Обучите несколько моделей**, включая как минимум одну LightGBM и одну не основанную на бустинге. Попробуйте разные гиперпараметры.
5. **Проанализируйте время обучения, время предсказания и качество моделей**.
6. **Выберите лучшую модель** по критериям заказчика и проверьте её качество на тестовой выборке.

### Примечания:
- В качестве метрики используйте **RMSE**.
- **Изучите библиотеку LightGBM** и используйте её для построения модели градиентного бустинга.
- Замеряйте время выполнения кода для обучения и предсказания модели.
- Градиентный бустинг может долго обучаться, поэтому меняйте только **2-3 параметра**.
- Если Jupyter Notebook начинает тормозить, удаляйте ненужные переменные:
  ```python
  del features_train
  ```

## Описание данных
Данные находятся в файле `/datasets/autos.csv`. В нём представлены следующие признаки:

| Признак | Описание |
|---------|-------------|
| `DateCrawled` | Дата скачивания анкеты из базы |
| `VehicleType` | Тип кузова автомобиля |
| `RegistrationYear` | Год регистрации автомобиля |
| `Gearbox` | Тип коробки передач |
| `Power` | Мощность двигателя (л.с.) |
| `Model` | Модель автомобиля |
| `Kilometer` | Пробег (км) |
| `RegistrationMonth` | Месяц регистрации автомобиля |
| `FuelType` | Тип топлива |
| `Brand` | Марка автомобиля |
| `Repaired` | Была ли машина в ремонте |
| `DateCreated` | Дата создания анкеты |
| `NumberOfPictures` | Количество фотографий автомобиля |
| `PostalCode` | Почтовый индекс владельца |
| `LastSeen` | Дата последней активности пользователя |

### Целевой признак:
- `Price` — Цена автомобиля (в евро)

## Критерии оценки
Ревьюеры проверяют:
- Выполнение всех шагов инструкции
- Подготовку данных
- Рассмотренные модели и гиперпараметры
- Отсутствие дублирования кода
- Выводы и их обоснованность
- Структуру проекта
- Чистоту и аккуратность кода

