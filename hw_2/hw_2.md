### Домашнее задание 2 - 10 баллов + 2 бонусных

В этом задании вам предстоит воспроизвести и обучить одну из самых знаменитых архитектур среди CV-моделей - AlexNet.

Данная модель была представлена в статье [ImageNet Classification with Deep Convolutional
Neural Networks](https://proceedings.neurips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf).

Подробное описание архитектуры приведено в секции статьи `3.5 Overall Architecture`.

1. Загрузите и подготовьте данные к обучению - **2 балла**
  - В отличие от оригинальной статьи, в данном задании модель будет применятся для классификации изображений из датасета [CIFAR100](https://pytorch.org/vision/main/generated/torchvision.datasets.CIFAR100.html#torchvision.datasets.CIFAR100) - загрузите его из torchvision, разделите датасет на обучающую, валидационную и тестовую выборки.
2. Реализуйте класс модели AlexNet для решения задачи и обучите ее, продемонстрировав уменьшение функции потерь на train/validation данных, а также измерьте релевантную, на ваш взгляд метрику классификации на test-части данных - **8 баллов**


**Общее**

Обеспечена воспроизводимость решения: зафиксированы random_state, ноутбук воспроизводится от начала до конца без ошибок - **1 балл**


**Дополнительные баллы**

Все, описанное выше, реализовано на pytorch lightning - **2 балла**

