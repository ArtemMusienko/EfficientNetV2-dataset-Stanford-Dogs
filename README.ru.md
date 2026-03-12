![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)

## EfficientNetV2 + dataset Stanford Dogs

**EfficientNetV2** — это усовершенствованное семейство нейронных сетей для компьютерного зрения, разработанное Google как развитие EfficientNet. Оно сочетает новые типы сверточных блоков (Fused-MBConv) и стратегию прогрессивного обучения, что делает тренировку моделей значительно быстрее, а сами модели — более точными и эффективными по сравнению с предыдущими версиями. Эти модели широко используются как готовые основы для задач классификации, детекции и сегментации изображений.

Данное решение демонстрирует использование тонкой настройки модели с помощью **EfficientNetV2** на примере набора данных **[Stanford Dogs](https://storage.yandexcloud.net/academy.ai/stanford_dogs.zip)**. 

Для достижения более лучшего результата были реализованы 3 callbacks: **EarlyStopping**, **ModelCheckpoint** и **ReduceLROnPlateau**. Также была применена техника аугментация, которая позволила достичь высоких результатов. Для ускорения вычислений на **GPU** будем использовать технику `mixed precision` (смешанной точности).

Финальная точность после дообучения: 
 - *Обучающая* выборка: 0.79;
 - *Валидационная* выборка: 0.87;
 - *Тестовая* выборка: 0.86.

> Настоятельно рекомендую использовать **графический ускоритель T4** или лучше!
