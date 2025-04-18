# Toxic Comment Classification for Wikishop

## Project Overview
This project was developed as part of a machine learning training course. The goal is to create a model capable of detecting toxic comments in a collaborative product description editing platform for the online store "Wikishop". Users can edit product descriptions and leave comments on others' changes. A moderation tool is required to automatically flag toxic comments.

## Task
Train a model to classify comments as either toxic or non-toxic. The dataset provided includes comments and toxicity labels. The performance target is an F1-score of at least 0.75.

## Dataset
- File: `/datasets/toxic_comments.csv`
- Features:
  - `text`: comment content
  - `toxic`: target label (1 - toxic, 0 - not toxic)

## Project Structure
1. Load and preprocess the data
2. Train various models
3. Evaluate and compare model performance
4. Choose the best model and draw conclusions

## BERT Note
If BERT is used:
- The project should be run locally due to memory limitations in the training environment (Jupyter notebook has only 4 GB RAM)
- Mention BERT in the project title in the first code cell

BERT is optional. The task can be solved using traditional ML or DL methods.

## Review Process
Projects are reviewed with attention to:
- Compliance with the project instructions
- Data preprocessing quality
- Model selection and hyperparameter tuning
- Code redundancy and structure
- Quality of conclusions
- Code cleanliness and structure

---

# Классификация токсичных комментариев для Викишоп

## Описание проекта
Проект разработан в рамках курса по машинному обучению. Цель — создать модель, способную выявлять токсичные комментарии в новой системе редактирования описаний товаров на платформе «Викишоп». Пользователи могут предлагать правки и оставлять комментарии к изменениям. Необходим инструмент для автоматической модерации токсичных сообщений.

## Задача
Обучить модель классифицировать комментарии как токсичные и нетоксичные. В наличии размеченный датасет. Целевое значение метрики F1 — не менее 0.75.

## Датасет
- Файл: `/datasets/toxic_comments.csv`
- Столбцы:
  - `text`: текст комментария
  - `toxic`: целевой признак (1 — токсичный, 0 — нет)

## Структура проекта
1. Загрузка и предобработка данных
2. Обучение различных моделей
3. Оценка и сравнение результатов
4. Выбор лучшей модели и формулирование выводов

## Примечание по BERT
Если используется BERT:
- Проект нужно выполнять локально (в Jupyter-ноутбуке ограничение по ОЗУ — 4 ГБ)
- Укажите BERT в заголовке проекта в первой ячейке

Использование BERT не обязательно. Задачу можно решить классическими ML или DL методами.

## Проверка проекта
Проект оценивается по следующим критериям:
- Соответствие инструкции
- Качество подготовки данных
- Выбор моделей и подбор гиперпараметров
- Отсутствие дублирования кода
- Качество выводов
- Структура и чистота кода
