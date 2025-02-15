# linear_algebra_bikesrent_analytics  🚀

# 1. Разделение данных на предикторы и целевую переменную 

#### Шаги выполнения 🎯:

1. Датасет загружается и обрабатывается, удалены мультиколлинеарные признаки (например, `atemp` из-за высокой корреляции с `temp`).
2. Разделение данных:
   - **Предикторы (X):** все столбцы, кроме `cnt`.
   - **Целевая переменная (y):** столбец `cnt`.
3. Данные делятся на обучающую и тестовую выборки (80% / 20%).

---

### 2. Реализация линейной регрессии 📈

Мы реализуем линейную регрессию по формуле наименьших квадратов:

#### Шаги выполнения:

1. Добавляем единичный столбец к данным (для учета свободного члена).
2. Рассчитываем коэффициенты регрессии с помощью матричных операций.
3. Реализуем метод предсказания.

---

### 3. Оценка качества модели 🏆

Для оценки качества модели используем две метрики:

1. **Среднеквадратичная ошибка (MSE):**
   - Показывает средний квадрат разности между фактическими и предсказанными значениями.

2. **Коэффициент детерминации (R²):**
   - Показывает, насколько хорошо модель объясняет вариативность данных.

**Результаты:**

- MSE: 693530.05 (чем меньше, тем лучше)
- R²: 0.827 (приближение к 1 говорит о хорошей модели)

---

### 4. Визуализация результатов 🎨

#### Фактические vs. предсказанные значения

- Сравнение реальных и предсказанных значений.

#### Гистограмма ошибок (остатков)

- Анализ распределения ошибок модели.

---

### 5. Выводы 📊

- Реализованная модель линейной регрессии показала хорошее качество с коэффициентом детерминации R² = 0.827.
- Температура (`temp`) является самым важным фактором, влияющим на спрос на велосипеды.
- Модель может быть улучшена за счет добавления полиномиальных признаков или использования нелинейных методов.

---

#### Библиотеки

- Python 3.x
- NumPy
- Matplotlib
- Pandas

![1](01.png)
![2](1.png)
![3](2.png)
