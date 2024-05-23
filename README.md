# Cats vs Dogs Prediction CNN Model

Download dataset from: https://www.kaggle.com/datasets/karakaggle/kaggle-cat-vs-dog-dataset <br>
<i>Make sure to use only the folder "PetImages".</i>

<hr>

I've built a CNN model that is able to distinguish between cats and dogs with an 81% accuracy. Furthermore, with 10 epochs I managed to reduce the loss and validation loss significantly while preventing
overfitting. Now, the CNN model can successfully predict a dog and a cat from the knowledge it has. Our dataset consists of approximately 25k images equally split among the 2 classes.

Imported modules:
<li>Pandas</li>
<li>Numpy</li>
<li>os</li>
<li>Tensorflow</li>
<li>Matplotlib</li>

<br>

Firstly, I converted our dataset into a DataFrame using pandas, with 2 columns: Images and Labels. I had to store the images as their relative paths and gave them their respective Label (0=cat, 1=dog).
The next step was to split the dataset into training and testing with an 80:20 split. After splitting our data, I performed augmentation and pre-processing using ImageDataGenerator from the TensorFlow
library.

Time to build our model! The model consists of 3 2D Convolution layers, 3 2D Max Pooling layers, Flatten Layer, and Dense layers. Moving forward, we define our optimizer as 'adam', loss, and metrics.
This way we bring our model to completion.

# Evaluation
The following graphs show the accuracy and loss throughout the 10 epochs.
![image](https://github.com/HarshaBeth/Cats-VS-Dogs/assets/92636321/3f7e49ae-34b6-4f52-ae01-d8bf6ab1199c)
![image](https://github.com/HarshaBeth/Cats-VS-Dogs/assets/92636321/7f42fe42-d3c0-4128-882d-ad51282e6a07)

# Prediction
Given such great results it was time to test our model, I chose a random image from our dataset and let the model predict. Below is an example!

![image](https://github.com/HarshaBeth/Cats-VS-Dogs/assets/92636321/f1392e9c-f63d-4606-b95b-791dd896c928)

