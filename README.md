# Classification of Handwritten Digits



## Abstract:

### Problem statement:

Image recognition is the process of identifying and detecting an object or a feature in a digital image or video. And the handwritten digits is a very basic trim of the area which can help us build up the understanding of how all the classifiers work and what are the theory fundamentals behind them. 

So the goal of this project is trying to use some of unsupervised and supervised classifiers learned from lectures including KNN, random forest, naïve Bayes, etc to recognize the handwritten digits from different people and different ways of writing. Then I will compare the performance of those methods as well as the efficiency or the strength and weakness of each method by using some common evaluation methods.

### Data description:

The data comes from an ongoing Kaggle competition. 

The data files contains test data and training data which are gray-scale images of hand-drawn digits, from zero through nine. Each image is 28 pixels in height and 28 pixels in width, for a total of 784 pixels in total. Each pixel has a single pixel-value associated with it, indicating the lightness or darkness of that pixel, with higher numbers meaning darker. This pixel-value is an integer between 0 and 255, inclusive.

Each pixel column in the training set has a name like $ pixelx$, where $x$ is an integer between 0 and 783, inclusive. To locate this pixel on the image, suppose that we have decomposed $x$ as $x = i * 28 + j$, where $i$ and  are integers between 0 and 27, inclusive. Then $pixelx$ is located on row $i$ and column $j$ of a 28 x 28 matrix, (indexing by zero).For example, $pixel31$ indicates the pixel that is in the fourth column from the left, and the second row from the top, as in the ascii-diagram below.

### Method plan:

Generally, I will use python to realize all the algorithms and especially work with *scikit learn* to build up the model, and *matplotlib* to visualize data. The number of the model to be used could change a little based on the time but overall I will cover all basic steps.

1. **Data processing**

   - Check the missing value
   - Normalize the data or do any necessary transformation on the data.
   - Split the data to training data and test data.
   
2. **Visualize the data (*matplotlib*)**:

   Check the features of the data and get a general idea of what I am gonna deal with.

3. **Establish model (*sklearn*):**

   (In this step, I will also tune on some parameters if it is necessary.)

   - KNN

   - Naive Bayes

   - Random forest

   - SVM

   - Logistic regression

   - More classification models if time permits.

4. **Make prediction on test data.**

### Evaluation Plan:

1. **Evaluation curves:**
   - ROC curve
   - PR curve
2. **Get the confusion matrices based on the validation data.**
