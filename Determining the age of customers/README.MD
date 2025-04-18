# Age Prediction Using Computer Vision

## 🛒 Project Overview

As part of the digital transformation at the retail chain **Khleb-Sol'**, I implemented a computer vision system for **automatic age estimation** based on customer photos. This solution is designed to:

- 🛍️ Analyze customer purchases and recommend products tailored to specific age groups.
- 🚫 Ensure compliance by preventing alcohol sales to underage individuals.

---

## 🧠 Project Steps

1. **Exploratory Data Analysis**  
   Analyzed a dataset of facial photographs annotated with ages.

2. **Data Preparation**  
   Applied preprocessing techniques to get the data ready for training.

3. **Model Training**  
   Built and trained a neural network to estimate age from facial images.

---

## 📊 Model Analysis

The model is built on top of the **ResNet50** architecture, enhanced with custom layers for regression:

### 🔧 Model Architecture

- `GlobalAveragePooling2D` — reduces spatial dimensions, preventing overfitting.  
- `Dense` — single neuron with ReLU activation for outputting age.

### 📈 Model Parameters

- Total parameters: `23,589,761`  
- Trainable parameters: `23,536,641`  
- Non-trainable (frozen) ResNet50 parameters: `53,120`

### 🚀 Training Details

- **Epochs:** 11  
- **Optimizer:** Adam  
- **Learning rate:** 0.0001  
- **Loss function:** Mean Squared Error (MSE)  
- **Metric:** Mean Absolute Error (MAE)

### 📉 Training Dynamics

- **Train MAE:** Improved from `12.31` → `2.65`  
- **Validation MAE:** Improved from `15.46` → `6.70`

> ✅ Target MAE < 8 achieved successfully.

---

## ✅ Conclusion

- The model meets the technical requirement:  
  **Validation MAE = 6.70 < 8**
- Shows strong convergence — errors steadily decrease.  
- No signs of overfitting — the gap between training and validation errors is minimal.

---

## 🔧 Suggestions for Improvement

- **Data Augmentation:**  
  Use light rotations to teach robustness to small angle changes.
  
- **Image Standardization:**  
  Normalize lighting and alignment to improve model performance.

- **Dataset Expansion:**  
  A larger dataset would enhance generalization.

- **Advanced Architecture:**  
  Using **EfficientNetB4** could improve both accuracy and speed.  
  However, the current environment is limited to **TensorFlow 2.1**, which prevents its use.

---

# _________________________

# Предсказание возраста с помощью компьютерного зрения

## 🛒 Описание проекта

В рамках цифровизации сети супермаркетов **«Хлеб-Соль»**, я внедрил систему компьютерного зрения для **автоматического определения возраста** по фотографии клиента. Это позволяет:

- 🛍️ Анализировать покупки и рекомендовать товары для нужной возрастной группы.
- 🚫 Контролировать продажу алкоголя, исключая обслуживание несовершеннолетних.

---

## 🧠 Этапы проекта

1. **Анализ данных**  
   Исследован набор фотографий с аннотированным возрастом.

2. **Подготовка данных**  
   Проведена предобработка и подготовка данных для обучения.

3. **Обучение модели**  
   Построена и обучена нейросеть для оценки возраста по фото.

---

## 📊 Анализ модели

В основе модели лежит предобученная **ResNet50**, дополненная слоями для регрессии:

### 🔧 Архитектура модели

- `GlobalAveragePooling2D` — усреднение по пространству, уменьшает переобучение.  
- `Dense` — один нейрон с ReLU для предсказания возраста.

### 📈 Параметры модели

- Всего параметров: `23,589,761`  
- Обучаемых: `23,536,641`  
- Необучаемых (замороженные слои ResNet50): `53,120`

### 🚀 Обучение

- **Эпохи:** 11  
- **Оптимизатор:** Adam  
- **Learning rate:** 0.0001  
- **Функция потерь:** Среднеквадратичное отклонение (MSE)  
- **Метрика:** Средняя абсолютная ошибка (MAE)

### 📉 Динамика обучения

- **Train MAE:** Снизилась с `12.31` до `2.65`  
- **Validation MAE:** Снизилась с `15.46` до `6.70`

> ✅ Целевое значение MAE < 8 успешно достигнуто.

---

## ✅ Выводы

- Модель соответствует требованиям:  
  **MAE на валидации = 6.70 < 8**
- Хорошая сходимость — ошибка стабильно снижается.  
- Переобучения не наблюдается — разница между train и validation MAE минимальна.

---

## 🔧 Возможные улучшения

- **Аугментация:**  
  Использовать небольшие повороты, чтобы повысить устойчивость к положению лица.

- **Стандартизация:**  
  Выравнивание освещения, смещений и поворотов улучшит результаты.

- **Увеличение датасета:**  
  Больше данных — лучше обобщение.

- **Продвинутая архитектура:**  
  **EfficientNetB4** дал бы идеальный баланс скорости и точности,  
  но он недоступен в текущей среде (TensorFlow 2.1).

---
