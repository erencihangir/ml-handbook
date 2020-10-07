<div align="center">
<img src="./imgs/shad.png"  width="300">
</div>
## Содержание учебника

Введение
 на примере прикладной задачи вводятся такие понятия как
обучающая выборка
вектор признаков
типы задач ML (supervised и unsupervised)
модель
метрика качества и функционал потерь
переобучение и методы борьбы с ним (разделение на train/test)
Показывается общий пайплайн решения задачи (от постановки, сбора данных и их очистки до оценки качества)
Линейные модели и вероятностный подход к ML
Задача Ordinary Least Squares, 
Аналитический вывод решения 
Численное решение.  (GD и SGD, их сходимость).
Вероятностная интерпретация OLS. 
Регуляризации l1 и l2. Зачем они нужны
Способы решения OLS с разной регуляризацией 
Logistic regression.
Вероятностная интерпретация задачи
(?) Метод ньютона (или унести в отдельный раздел по SGD)
Generalized linear regression
Exponential family distributions
OLS, logreg, softmax и poisson как частные случаи GLM. 
Generative approach ; Naive bayes
Генеративный и дискриминативный подходы к обучению
GDA
Linear Discriminant Analysis
Метод наивного байеса (хорошая глава из книги)
Связь между логистической регрессией и методом наивного Байеса
Как программировать линейные модели
Vowpal wabbit
Parameter server
Взвешенные выборки
пропуски в данных, sparse данные, категориальные признаки
Современное около линейных моделей (неглубоко и со ссылками)
Regularized dual averaging
FTRL

Деревья решений и бустинг 
тут предлагаю игнорировать Adaboost/brownboost итд и сразу выводить к катбусту/lightgbm
Инженерный подход к построению классификаторов и регрессоров
Деревья решений
Энтропия, information gain, gini, variance reduction
Алгоритм C4.5, CART, CHAID, Mars
Оптимизация дифференцируемых метрик деревьями
Регуляризация деревьев
Random forest
Bias - Variance tradeoff
Бэггинг
Градиентный бустинг
Построение для MSE
Построение в общем виде для дифференцируемой ошибки
Метод ньютона
Классификация на деревьях
Как программировать
Алгори    тмическая сложность построения дерева
Гистограммный метод построения https://github.com/microsoft/LightGBM/blob/master/docs/Features.rst
ODT
Параллелизм
CatBoost, Xgboost, LightGBM
Примеры в индустрии, Яндекс
Метрические алгоритмы
KNN
Поиск ближайшего соседа, объяснить как связан с поиском и рекомендациями
HNSW
FAISS / SCANN (link)
    
Практические вопросы
Кросс-валидация
Holdout Cross Validation
K-fold Cross Validation
Bias-Variance (как вот тут http://www.it.uu.se/edu/course/homepage/sml/lectures/lecture5_handout.pdf)
Leave One Out
Cross Validation for Time Series
Ограничения использования кросс-валидации (пример на тему того, что трейн и тест должны быть из одного распределения) и tricky cases (такой как кросс-валидация на признаках со статистической информацией)
Техники подбора гиперпараметров
Grid Search
Random Search + Early Stopping Algorithms (SHA)
Bayesian Optimization
Tree of Parzen Estimators
Evolutionary optimization
Open source библиотеки (Hyperopt)
Предобработка данных
Заполнение пропусков: заполнение константой, kNN, MICE(?), SVD(?)
Нормализация данных: Standart Scaling, MinMaxScaling
Работа с выбросами в данных
Предобработка категориальных и порядковых признаков
Feature Extraction
Извлечение фич из картинок (с отсылкой к курсу CV)
Из текстов: BoW, Tf-Idf, Word Embeddings (с отсылкой к курсу NLP)
Сумасшедшие примеры (геометки, даты и так далее и какие признаки можно на их основе конструировать)
Признаки-счётчики, примеры группировки фич
Feature Selection
Greedy Selection: forward, backward
Статистические методы отбора
l1 регуляризация для отбора фичей
Метрики
Бинарная классификация: Accuracy, ROC-AUC, Precision, Recall, F1-мера
Multilabel, multiclass классификация
Регрессия: MAE, RMSE, MAPE (с отсылкой к курсу практический DS)
Ранжирование/рекомендации

Инструменты
Джентльменский набор библиотек
Библиотеки numpy, sklearn, основное
Библиотека pandas, основное: типы данных, индексирование, merge, частые функции (например, apply)
Advanced numpy, pandas: решение задач вида “как с помощью одной функции из библиотеки сделать … ”
Разведочный анализ данных
Набор задач и хороших визуализаций для них 
Обзор и сравнение библиотек для визуализации данных
Tensorflow / pytorch (?)
VW, catboost
