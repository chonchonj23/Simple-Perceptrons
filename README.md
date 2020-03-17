Here are three simple perceptrons and linear perceptron algorithm that had been taught in Udacity's Machine Learning Nanodegree.

Perceptrons contain an activation function (which can be interpreted as some sort of mapping function) that transforms inputs into certain output value based on specific activation rule.

For the three perceptrons, feel free to change the weights and bias in the Python programs, and see what happens. 
Note that test_inputs array is given, and correct_outputs array comes directly from perceptron activation, which in turn is defined via the weights and bias that we can adjust in these two simple examples.

For the linear perceptron algorithm, note that:
- we are using X1 and X2 to predict Y ( via a step function )
- If a point is correctly classified, do nothing
- If a point (e.g. with coordinates X1,X2) is wrongly classified, do one of the following: 
  => If the point is classified positive, but it has a negative label, subtract αX1, αX2, and α from the weights (e.g. w1 & w2) and bias term (e.g. b) respectively, given that we are at the point (X1,X2)
  => If the point is classified negative, but it has a positive label, add αX1, αX2, and α to the weights (e.g. w1 & w2) and bias term (e.g. b) respectively, given that we are at the point (X1,X2)
  => α is the learning rate
