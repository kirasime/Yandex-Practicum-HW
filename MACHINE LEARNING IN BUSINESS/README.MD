# Choosing the Best Oil Well Location

## Problem Statement
The oil extraction company "GlavRosGosNeft" is looking for the optimal location to drill a new well. The challenge is to determine which region will yield the highest profit based on existing geological survey data.

### Task Overview
You have access to oil sample data from three regions. Each region contains information on oil well characteristics and the volume of reserves. Your goal is to develop a model that predicts the amount of oil in each well and to determine the most profitable region for drilling. Additionally, you will analyze potential profits and risks using the Bootstrap technique.

### Key Conditions:
- The dataset includes three regions, each with multiple oil well data points.
- The **only suitable model** for training is **linear regression** (other models do not provide reliable predictions).
- In each region, **500 wells** are surveyed, and machine learning selects **the top 200** for development.
- The total budget for developing wells in a region is **10 billion rubles**.
- The revenue per barrel of oil is **450 rubles**, which translates to **450,000 rubles per unit of product** (since reserves are measured in thousands of barrels).
- A region is only considered viable if the probability of financial losses is **less than 2.5%**.
- Among the viable regions, the one with the **highest average profit** will be selected.

### Dataset Description
The geological survey data for the three regions is available in the following files:
- `/datasets/geo_data_0.csv`
- `/datasets/geo_data_1.csv`
- `/datasets/geo_data_2.csv`

The dataset contains the following features:

| Feature | Description |
|---------|-------------|
| `id` | Unique identifier of the oil well |
| `f0`, `f1`, `f2` | Three key features of each location (details are not provided, but they are significant for predictions) |
| `product` | Oil reserve volume in the well (thousands of barrels) |

### Required Analysis Steps
1. **Data Preparation:** Load and clean the data, handle missing values, and analyze distributions.
2. **Model Training and Evaluation:**
   - Split the dataset into **training (75%)** and **validation (25%)** sets.
   - Train a **linear regression model** for each region.
   - Make predictions on the validation set and calculate **RMSE**.
   - Compare predicted vs. actual reserves and analyze performance.
3. **Profit Calculation:**
   - Determine the **minimum required oil reserves** for a well to be profitable.
   - Compare this threshold with the **average predicted reserves** for each region.
   - Summarize key insights from this analysis.
4. **Profit Estimation Using Model Predictions:**
   - Select the **top 200 wells** with the highest predicted reserves.
   - Compute the total **actual oil reserves** for these wells.
   - Calculate **expected profit** based on the total reserves.
5. **Risk Assessment with Bootstrap:**
   - Use **Bootstrap sampling (1000 iterations)** to estimate the **distribution of profits**.
   - Calculate **mean profit, 95% confidence interval, and risk of financial loss**.
   - Identify regions where the **loss probability is below 2.5%** and select the most profitable one.

### Expected Outcomes
- **Identify the region with the highest expected profit** while maintaining an acceptable level of risk.
- **Provide insights into financial feasibility**, including the break-even oil reserve volume per well.
- **Use statistical analysis to justify the final recommendation**.

### Evaluation Criteria
Your project will be assessed based on:
- The completeness and correctness of the **data preparation**.
- Proper **implementation of model training and validation**.
- Consideration of all **business constraints**.
- **Statistical soundness** of the Bootstrap risk analysis.
- A well-supported **recommendation for the best drilling location**.
- **Code efficiency and structure** (avoidance of redundancy, clarity, and maintainability).

---

# Выбор наилучшей локации для бурения нефтяной скважины

## Описание задачи
Нефтедобывающая компания "ГлавРосГосНефть" ищет оптимальное место для бурения новой скважины. Необходимо определить, какой регион принесет наибольшую прибыль, основываясь на данных геологоразведки.

### Постановка задачи
У вас есть данные о пробах нефти из трех регионов. В каждом регионе содержится информация о характеристиках нефтяных скважин и объеме запасов. Ваша цель – построить модель, которая прогнозирует объем нефти в каждой скважине, и определить наиболее прибыльный регион для бурения. Кроме того, необходимо проанализировать возможную прибыль и риски с использованием техники Bootstrap.

### Основные условия:
- В каждом регионе исследуется **500 скважин**, из которых **200 лучших** отбираются с помощью машинного обучения.
- В качестве модели допускается **только линейная регрессия**.
- Бюджет на разработку скважин в одном регионе – **10 миллиардов рублей**.
- Цена за баррель нефти составляет **450 рублей** (то есть **450 000 рублей за 1000 баррелей**).
- Регион может быть выбран только в том случае, если вероятность убытков составляет **менее 2.5%**.
- Среди регионов, удовлетворяющих этому условию, выбирается **регион с наибольшей средней прибылью**.

### Описание данных
Геологоразведочные данные по трем регионам находятся в файлах:
- `/datasets/geo_data_0.csv`
- `/datasets/geo_data_1.csv`
- `/datasets/geo_data_2.csv`

Датасет содержит следующие признаки:

| Признак | Описание |
|---------|-------------|
| `id` | Уникальный идентификатор скважины |
| `f0`, `f1`, `f2` | Три ключевых признака точки (их смысл не уточняется, но они важны для предсказаний) |
| `product` | Объем запасов нефти в скважине (тыс. баррелей) |

### Этапы анализа
1. **Подготовка данных:** загрузка, очистка, обработка пропусков, анализ распределений.
2. **Обучение и оценка модели:**
   - Разделение данных на **обучающую (75%)** и **валидационную (25%)** выборки.
   - Обучение модели **линейной регрессии**.
   - Предсказание и расчет **RMSE**.
   - Анализ результатов.
3. **Расчет прибыли:**
   - Определение **минимально необходимого объема нефти** для безубыточности.
   - Сравнение порогового значения с **средними предсказанными запасами**.
   - Выводы по анализу.
4. **Оценка прибыли по предсказаниям модели:**
   - Выбор **200 лучших скважин**.
   - Подсчет общего **объема нефти**.
   - Расчет **ожидаемой прибыли**.
5. **Анализ рисков с Bootstrap:**
   - Проведение **1000 итераций Bootstrap**.
   - Определение **средней прибыли, доверительного интервала и вероятности убытков**.
   - Выбор **наиболее прибыльного и безопасного региона**.

### Итог
- **Определение наиболее прибыльного региона** при минимальном уровне риска.
- **Оценка финансовой целесообразности** бурения.
- **Статистическое обоснование выбора**.
