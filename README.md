# Google Collab link:
https://colab.research.google.com/drive/1G2YxjVkGqK-1Q1Ar8ceZhfANqGpcjNbe?usp=sharing

# Fashion-MNIST-Image-Classification


### 1. What is the Fashion MNIST dataset?

Fashion-MNIST is a popular dataset used to teach and test image-classification models, and you can think of it as MNIST’s more realistic cousin. Instead of handwritten digits, it contains 70,000 small grayscale images of everyday clothing items like T-shirts, shoes, and bags, each sized 28×28 pixels and grouped into 10 categories. It was created by Zalando Research to be easy to use while still being challenging enough to reflect real-world problems, which is why it’s often used by students and researchers to practice building and comparing machine-learning models.

### 2. Why do we normalize image pixel values before training?

We normalize image pixel values before training because it makes learning easier and more stable for the model. Raw pixel values (usually 0–255) can be large and unevenly scaled, which can slow down training and make optimization harder. By scaling them to a smaller range (like 0–1 or −1 to 1), the model’s gradients behave more predictably, helping it converge faster and avoid numerical issues. Normalization also ensures that all input features are on a similar scale, so no single pixel dominates the learning process just because of its magnitude.


### 3. List the layers used in the neural network and their functions.

Flatten layer: Converts the 2D image into a 1D array.

Dense (hidden) layer: Learns patterns and relationships in the data.

ReLU activation: Adds non-linearity to help learn complex features.

Output layer (Softmax): Outputs probabilities for each clothing class.


### 4. What does an epoch mean in model training?

An epoch is one complete pass through the entire training dataset.
During one epoch, the model sees every training example once.
Multiple epochs allow the model to gradually improve its accuracy.

### 5. Compare the predicted label and actual label for the first test image.

The actual label is the true clothing category from the dataset.
The predicted label is the category chosen by the model.
If both labels are the same, the prediction is correct; otherwise, it is incorrect.
(Example: Actual label = “Sneaker”, Predicted label = “Sneaker” → Correct)

### 6. What could be done to improve the model’s accuracy?

Train the model for more epochs

Add more hidden layers or neurons

Use data augmentation

Adjust the learning rate or batch size

Apply regularization techniques like dropout
