# Age and Gender Detection Cross Entropy vs Ordinal vs CORAL
This project is performed using **Pytorch and ResNet-34** is used as backbone. The Datasets used were **UTKFace and MORPH-2**. The face images were **cropped and preprocessed**. It is split into **Train-Validation-Test sets(80-10-10)**. The Images are labeled in .csv files. The **Batch size** used is **256**.

![Cross Entropy](https://github.com/Chirag-Sai-Panuganti/Age-and-Gender-Detection-Cross-Entropy-vs-Ordinal-vs-CORAL/blob/main/Architectures/Cross%20Entropy.JPG)

This is the **Cross Entropy Architecture**.The **Soft max layer** is applied in the final layer.The Optimizer used was **ADAM** and the **learning Rate is 0.0005**. The **Accuracy of Gender** is **83.78%(UTKFace) and 99.18%(MORPH-2)** and **Mean Absolute Error for Age** is **7.13(UTKFace) and 3.27(MORPH-2)**.

![CORAL](https://github.com/Chirag-Sai-Panuganti/Age-and-Gender-Detection-Cross-Entropy-vs-Ordinal-vs-CORAL/blob/main/Architectures/CORAL.JPG)

This is **Consistent Ranked Logits(CORAL) Architecture**.The **n-1 indvidual classifiers** are applied in the final layer.The Optimizer used was **ADAM** and the loss function is **Weighted Cross Entropy Loss Function**.The **learning rate is 0.0005**. The **Accuracy of Gender** is **89.20%(UTKFace) and 99.38%(MORPH-2)** and **Mean Absolute Error for Age** is **5.58(UTKFace) and 2.57(MORPH-2)**.
