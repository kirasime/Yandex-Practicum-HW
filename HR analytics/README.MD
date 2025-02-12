## Employee Turnover and Satisfaction Prediction

### Project Description
This project focuses on HR analytics to help businesses optimize workforce management. The goal is to develop machine learning models that predict:

1. **Employee satisfaction level** based on company-provided data.
2. **Employee turnover likelihood** to reduce unexpected resignations.

By leveraging predictive analytics, businesses can mitigate financial risks associated with workforce attrition.

### Task 1: Predicting Employee Satisfaction
The dataset includes the following features:
- `id`: Unique employee identifier
- `dept`: Department
- `level`: Job position level
- `workload`: Workload intensity
- `employment_years`: Years at the company
- `last_year_promo`: Whether the employee received a promotion last year
- `last_year_violations`: Any policy violations in the last year
- `supervisor_evaluation`: Supervisor's performance rating
- `salary`: Monthly salary
- `job_satisfaction_rate`: Target variable, satisfaction level (0 to 1 scale)

#### Workflow
1. **Data Loading**: Import training and test datasets.
2. **Preprocessing**: Handle missing values and prepare features.
3. **Exploratory Data Analysis (EDA)**: Investigate feature distributions.
4. **Feature Engineering**: Apply transformations and encoding.
5. **Model Training**: Train multiple models (linear regression, decision tree, etc.) and optimize hyperparameters.
6. **Evaluation**: Select the best model using SMAPE (Symmetric Mean Absolute Percentage Error) with a success criterion of SMAPE ≤ 15.
7. **Results & Insights**: Document findings and model performance.

### Task 2: Predicting Employee Turnover
The same feature set is used, but the target variable is `quit` (whether an employee leaves the company).

#### Workflow
1. **Data Loading**: Import datasets.
2. **Preprocessing**: Handle missing values and prepare data.
3. **EDA**: Identify turnover trends and correlations.
4. **Feature Addition**: Use predicted `job_satisfaction_rate` as an additional input feature.
5. **Model Training**: Train multiple models and optimize hyperparameters.
6. **Evaluation**: Assess models using ROC-AUC, with a success criterion of ROC-AUC ≥ 0.91.
7. **Results & Insights**: Document key findings.

### Final Summary
- Developed ML models for predicting employee satisfaction and turnover.
- Provided actionable insights to help businesses minimize employee attrition.
- Ensured structured data preprocessing and automation for reproducibility.

---

## Прогнозирование Увольнений и Удовлетворённости Сотрудников

### Описание Проекта
Этот проект посвящён HR-аналитике и помогает бизнесу оптимизировать управление персоналом. Задачи:

1. **Прогнозирование уровня удовлетворённости сотрудника** на основе данных компании.
2. **Предсказание вероятности увольнения сотрудника**, чтобы минимизировать неожиданные потери кадров.

Использование машинного обучения позволит компании снизить риски, связанные с оттоком сотрудников.

### Задача 1: Прогнозирование Удовлетворённости Сотрудника
Датасет включает следующие признаки:
- `id`: Уникальный идентификатор сотрудника
- `dept`: Отдел
- `level`: Уровень занимаемой должности
- `workload`: Загруженность
- `employment_years`: Количество лет работы в компании
- `last_year_promo`: Было ли повышение за последний год
- `last_year_violations`: Были ли нарушения трудового договора
- `supervisor_evaluation`: Оценка руководителя
- `salary`: Зарплата
- `job_satisfaction_rate`: Целевой признак, уровень удовлетворённости (от 0 до 1)

#### Этапы Работы
1. **Загрузка Данных**: Импорт обучающего и тестового датасетов.
2. **Предобработка**: Обработка пропущенных значений и подготовка данных.
3. **Исследовательский Анализ**: Анализ распределений и взаимосвязей признаков.
4. **Создание Признаков**: Кодирование и трансформация данных.
5. **Обучение Моделей**: Обучение нескольких моделей (линейная регрессия, решающее дерево и др.), настройка гиперпараметров.
6. **Оценка Качества**: Выбор лучшей модели на основе метрики SMAPE (≤ 15).
7. **Выводы и Инсайты**: Документирование результатов.

### Задача 2: Прогнозирование Увольнений
Используются те же признаки, но целевой переменной является `quit` (уволился / остался в компании).

#### Этапы Работы
1. **Загрузка Данных**: Импорт датасетов.
2. **Предобработка**: Обработка пропусков и очистка данных.
3. **Исследовательский Анализ**: Анализ закономерностей увольнений.
4. **Добавление Признака**: Включение предсказанного `job_satisfaction_rate` как нового признака.
5. **Обучение Моделей**: Обучение и настройка нескольких моделей.
6. **Оценка Качества**: Использование ROC-AUC (≥ 0.91) для выбора лучшей модели.
7. **Выводы и Инсайты**: Финальные наблюдения и рекомендации.

### Итог
- Разработаны модели для прогнозирования удовлетворённости и увольнений сотрудников.
- Даны рекомендации по снижению оттока персонала.
- Использован структурированный процесс обработки данных и автоматизация для воспроизводимости результатов.
