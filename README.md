# CNN
I built a Convolutional Neural Network to classify images of vegetables. The goal was to train a model that can look at an image and correctly identify what type of vegetable it is. This is useful because image classification is used in a lot of real-world things like food recognition apps and even automation in agriculture.”
The dataset I used was a vegetable image dataset that included different classes like beans, carrots, cucumbers, tomatoes, and others.”

Each class = a type of vegetable
Images stored in folders (one folder per class)
Important note:
Each class only had about 5 images

The model’s job was to take an image and predict which class it belongs to

Used image_dataset_from_directory
Ignored .ipynb_checkpoints folder

resized all images to 128 by 128 and grouped them into batches of 8

normalized the pixel values by dividing by 255 so all values are between 0 and 1

built a Convolutional Neural Network.”

Conv Layer 
ReLU
Max Pooling 

Conv2D (32 filters)
MaxPooling
Conv2D (64 filters)
Flatten
Dense (output layer)

compiled the model using:

Adam optimizer
Sparse categorical crossentropy 
Accuracy as the metric

trained the model for 10 epochs using training and validation data

plotted training and validation accuracy over time to see how well the model was learning

created a confusion matrix to see how well the model predicted each class.

After building the original model, I tried improving it by adding dropout
