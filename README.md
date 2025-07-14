# Deep-Learning
Deep Learning Project (CIFAR-100)

🎯 What Are We Trying to Achieve in This Project?
The core goal is to train a CNN (Convolutional Neural Network) from scratch using a subset of the CIFAR-100 image dataset to classify images into correct categories (like tree, bottle, keyboard, etc.). The project tests different CNN architectures, activation functions, optimizers, and training setups to find combinations that give better classification accuracy.

📁 1. What is the CIFAR-100 Data Set?
CIFAR-100 is a set of 60,000 tiny photographs, each of which is labelled with one of 100 categories, such as dog, bus, fish, or mountain.
The images are only 32x32 pixels, which is the size of a small stamp, and they are coloured, not black and white. We ask the computer, "Can you tell what's in this image?" It's like a visual test.
I have only chosen 10 out of 100 categories for training so it would be quick and easy. This is because we don't have powerful machines or a lot of RAM in free Google Colab.

 🧠2. What Does It Mean to "Train a CNN"?

 It is like training a system to look at thousands of example images and learn how to tell what each one shows by looking at patterns like shapes, edges, and colours.It operates the same way as training a new employee. We start by showing the system a lot of examples, such "this is a car" and "this is a ship." Over time, the system learns how to tell them apart on its own.

🔧  3. What were the tests that were done to make things more accurate?
You ran a number of tests to make the underlying model more accurate after it was working. We changed one thing for each test and then looked at what happened: 

✅ a) Make the Model Bigger (Deeper)
More layers mean more brain capacity.
Result: The accuracy became a little better, but there were too many layers, which made it too complicated (risk of overfitting).

✅ b) Use Different Functions to Turn On
These are basically the model's reasoning units that help it figure out whether something is important or not.
Best results: Tanh and Leaky ReLU
Worst: Sigmoid (too sluggish, doesn't learn well) 

✅ c) Try Different Optimisers
You may think of this as different ways to learn.
Best: Adam (quick and even)
RMSprop is the worst, especially if the learning rate is low. 

✅ d) Change the training settings, like the batch size and the number of epochs.
Batch size tells it how many pictures to learn from at once.
Epoch is the number of times it views the entire dataset.
Best outcomes: Batch size is 64 or 128, and there are about 15 to 20 epochs.

📊 4. How to Read Graphs, Charts, and Percentages ?
During model training, you will usually observe two main plots:
✅ A. Plot of accuracy (training vs. validation)
Shows how often predictions were right throughout time.
The model is learning if the accuracy goes up steadily.
If the training accuracy is high but the validation accuracy is low, the model is overfitting (it is remembering things instead of generalising them).

✅ B. Loss Graph
Tells you how erroneous the model is.
It's better to have less loss.
If loss keeps going down, the training is working.
The model can be overly complicated or confused if it goes up again.
Percentages (Accuracy %):
If accuracy is 70%, that means that 7 out of 10 forecasts were right.
For your project:
Base accuracy: about 65%
Better: Up to 71.4%
That's a good gain given the few resources available.

 🧾 5. A full summary of the project in plain English
I made an image recognition system from scratch and taught it how to tell what things are from pictures. I utilised the CIFAR-100 dataset, but I just used 10 categories to make it easier for the system. To figure out how to acquire the best accuracy, I tried out several designs and ways of learning. In the end, I was able to raise the accuracy from 65% to more than 71% by changing the size of the model, the learning settings, and the ways it was activated.

These tests taught me how to make smart systems better in the real world. These are the same systems used in medical diagnosis, facial recognition, and cybersecurity.


