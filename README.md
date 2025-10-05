   CIFAR-10 Image Classification

My name is Shrishti Yadav, a Computer Science (AIML) student at ABES Engineering College. This repository contains my implementation for the CIFAR-10 image classification assignment as part of the AIRL CV Intern task.
I worked on this project to strengthen my understanding of Convolutional Neural Networks (CNNs) and gain hands-on experience in building an image classification model from scratch.

Project Overview

The objective of this assignment was to classify images from the CIFAR-10 dataset, which consists of 60,000 32×32 color images divided into 10 classes such as airplane, automobile, bird, cat, and truck.

Instead of using pre-trained models, I built a custom CNN using TensorFlow/Keras to better understand how each component contributes to the model’s performance.

Tools and Technologies

Programming Language: Python

Framework: TensorFlow / Keras

Dataset: CIFAR-10

Tools Used: Google Colab, NumPy, Matplotlib

Approach

Data Preprocessing:
I began by loading the CIFAR-10 dataset from Keras and normalizing the pixel values from the range [0, 255] to [0, 1]. This helped the model train more efficiently.

Model Architecture:
I designed a CNN with three convolutional layers followed by max pooling. The output was then flattened and passed through fully connected layers with a softmax activation for multi-class classification.
To reduce overfitting, I used dropout layers and data augmentation.

Model Training:

Optimizer: Adam

Loss Function: Categorical Crossentropy

Batch Size: 64

Epochs: 20

Validation Split: 0.2

Hyperparameter Tuning:
Initially, my model accuracy was around 45–50%. After experimenting with deeper layers, data augmentation, and a lower learning rate, I achieved improved performance.

Results
Metric	Value
Training Accuracy	~65%
Validation Accuracy	~60%

Best Classification Accuracy on CIFAR-10: approximately 60%

While the accuracy is modest, it reflects a solid baseline for a model trained from scratch without pre-trained weights.

Challenges Faced and How I Solved Them

Slow Model Learning:
The model was not improving after several epochs. I realized the input data wasn’t normalized properly and fixed it, which improved training speed.

Overfitting:
Validation accuracy dropped after 10 epochs. I added dropout layers and applied image augmentation techniques like flipping and rotation to help the model generalize better.

Optimizer and Learning Rate:
I initially used SGD but switched to Adam optimizer with a lower learning rate, which stabilized training and improved accuracy.

Through each problem, I learned how tuning hyperparameters and understanding model behavior can significantly affect results.

Future Improvements

If I continue developing this model, I plan to:

Use transfer learning with architectures like ResNet or VGG to improve accuracy above 85%.

Add batch normalization for better gradient flow.

Implement learning rate scheduling for stable convergence.

Experiment with attention mechanisms to enhance feature extraction.

 

Author

Shrishti Yadav
Department of Computer Science (AIML)
ABES Engineering College
Email: yshrishti39@gmail.com
