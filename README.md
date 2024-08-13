Пояснения:
1)Загрузка данных: 
	Загружаем данные тренировочного (train.csv) и тестового (test.csv) наборов.

2)Предварительная обработка: 
	Заполняем пропущенные значения, преобразуем категориальные данные в числовые с помощью метода pd.get_dummies. Масштабируем данные с использованием StandardScaler.

3)Создание и компиляция модели: 
	Модель состоит из нескольких полносвязных слоев, с функцией активации relu. Для регуляризации используются слои Dropout. Последний слой имеет функцию активации sigmoid, поскольку 		задача бинарной классификации.

4)Обучение модели: 
	Модель обучается на обучающем наборе с использованием ранней остановки (EarlyStopping), чтобы предотвратить переобучение.

5)Оценка модели: 
	Оцениваем точность на валидационном наборе.

6)Предсказания:
	Делаем предсказания на тестовом наборе данных и сохраняем результаты в файл submission.csv для отправки на Kaggle.
