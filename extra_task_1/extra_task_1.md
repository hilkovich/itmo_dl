### Дополнительное задание 1 - 5 баллов

1. Загрузите датасет оценки качества воздуха в различных регионах - [air_quality.csv](https://disk.yandex.ru/d/29AVoENYZR4NyA)
2. Подготовьте данные к обучению - **1 балл**
  - Разделите датасет на обучающую, валидационную и тестовую выборки со стратификацией. В качестве целевой переменной используйте столбец `air_quality` - бинарный столбец (0 - плохое качество воздуха, 1 - хорошее качество воздуха).
  - Создайте объекты для работы с данными в PyTorch - `Dataset` и `DataLoader` для обучающей, валидационной и тестовой выборок. Выберите оптимальный, на ваш взгляд, `batch_size`.
3. Реализуйте класс нейросетевой модели для решения задачи - **1 балл**
  - Минимальное количество `Linear` слоев в структуре - 3 штуки: входной слой, скрытый слой, выходной классификационный слой.
  - Подберите оптимальные для задачи функции активации - `ReLU`, `Sigmoid`, `Tanh`, `LeakyReLU`...
  - Реализуйте логику прохождения данных по сети в методе `forward`
  - Cоздайте объект модели, реализуйте перевод модели на gpu
4. Напишите код цикла обучения - train-loop и валидации - eval-loop. В процессе обучения сохраняйте значения функции потерь на тренировочной и валидационной выборках - **1 балл**
5. Обучите модель и проверьте ее качество - **1 балл**
  - Выберите оптимизатор, в качестве функции потерь используйте `nn.BCELoss`
  - Запустите обучение, постарайтесь подобрать оптимальные скорость обучения и количество эпох, ориентируясь на динамику функции потерь на train/val
  - Измерьте качество лучшей модели на тестовой выборке, постройте отчет о классификации - `classification_report`

Обеспечена воспроизводимость решения: зафиксированы random_state, ноутбук воспроизводится от начала до конца без ошибок - **1 балл**