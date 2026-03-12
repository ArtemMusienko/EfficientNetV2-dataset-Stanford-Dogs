![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)![Google Colab](https://img.shields.io/badge/Google%20Colab-%23F9A825.svg?style=for-the-badge&logo=googlecolab&logoColor=white)

## EfficientNetV2 + dataset Stanford Dogs

 [![ru](https://img.shields.io/badge/README_на_русском-2A2C39?style=for-the-badge&logo=github&logoColor=white)](README.ru.md) 

**EfficientNetV2** is an advanced family of neural networks for computer vision developed by Google as an evolution of EfficientNet. It combines new types of convolutional blocks (Fused-MBConv) and a progressive training strategy, making model training significantly faster and more accurate and efficient than previous versions. These models are widely used as ready-made bases for image classification, detection, and segmentation tasks.

This solution demonstrates the use of fine-tuning the model using **EfficientNetV2** using the **[Stanford Dogs](https://storage.yandexcloud.net/academy.ai/stanford_dogs.zip)** dataset as an example.

 To achieve better results, 3 callbacks were implemented: **EarlyStopping**, **ModelCheckpoint**, and **ReduceLROnPlateau**. Augmentation techniques were also used to achieve high results. To speed up calculations on the **GPU**, we will use the `mixed precision` technique (mixed precision).

Final accuracy after fine-tuning:

- *Training* sample: 0.79;
- *Validation* sample: 0.87;
- *Test* sample: 0.86.

> I strongly recommend using a **T4 graphics accelerator** or better!