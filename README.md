# Titanic Survival Data Cleaning and Modeling

## Описание проекта

Этот проект посвящен анализу данных о пассажирах Титаника, с целью предсказания выживаемости пассажиров на основе доступных данных. Основное внимание уделяется очистке данных, обработке пропущенных значений, математическому преобразованию признаков и обучению модели классификации.

## Содержание

- [Описание проекта](#Описание-проекта)
- [Данные](#Данные)
- [Цель](#Цель)
- [Этапы работы](#Этапы-работы)
- [Метрики](#Метрики)
- [Выводы](#Выводы)
- [Использование](#Использование)

## Данные

В проекте используется датасет `train.csv`, содержащий данные о пассажирах Титаника. Этот файл включает такие признаки как:
- `PassengerId` - идентификатор пассажира
- `Survived` - целевой признак (1 - пассажир выжил, 0 - погиб)
- `Pclass` - класс пассажира
- `Name` - имя пассажира
- `Sex` - пол
- `Age` - возраст
- `SibSp` - количество братьев/сестер или супругов на борту
- `Parch` - количество родителей/детей на борту
- `Ticket` - номер билета
- `Fare` - плата за проезд
- `Cabin` - каюта
- `Embarked` - порт посадки

## Цель

Основная цель проекта — улучшить точность модели предсказания выживаемости пассажиров Титаника с помощью тщательной предобработки данных и последующего обучения модели логистической регрессии.

## Этапы работы

1. **Получение и загрузка данных:**  
   Загрузка данных и первичный анализ для выявления пропусков и категориальных переменных.

2. **Удаление пропущенных значений и категориальных переменных:**  
   Первичная очистка данных с удалением пропусков и категориальных переменных. Обучение модели на этих данных и оценка метрики качества.

3. **Повторная загрузка данных и их обработка:**  
   Заполнение пропусков различными методами, кодирование категориальных переменных и обучение модели на обработанных данных.

4. **Математическое преобразование признака `Age`:**  
   Применение различных методов преобразования признака `Age` и выбор наилучшего из них.

5. **Обучение модели на преобразованных данных:**  
   Обучение модели на данных после математического преобразования и оценка метрики качества.

6. **Визуализация и анализ результатов:**  
   Построение графиков для лучшего понимания данных и выводов, касающихся факторов, влияющих на выживаемость.

## Метрики

Для оценки качества модели использовалась метрика **точности (accuracy)**, которая позволяет измерить долю правильно классифицированных примеров среди всех предсказанных.

## Выводы

- Очистка данных и их правильное преобразование значительно улучшают точность модели.
- Модель, обученная на обработанных данных с математическим преобразованием признака `Age`, показала улучшение метрики на **10.74%** по сравнению с моделью, обученной на необработанных данных.

## Использование

Для запуска проекта:
1. Клонируйте репозиторий:
    ```bash
    git clone git@github.com:AlessioLoginov/Titanic-Survival-Data-Cleaning-and-Modeling.git
    ```
2. Убедитесь, что у вас установлены необходимые библиотеки:
    ```bash
    pip install -r requirements.txt
    ```
3. Запустите Jupyter Notebook и следуйте шагам в файле `Titanic_Survival_Analysis.ipynb`.


