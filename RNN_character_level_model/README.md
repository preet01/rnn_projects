## Character-level language model

This code implements multi-layer Recurrent Neural Network for training/sampling from character-level language models. In other words the model takes one text file as input and trains a Recurrent Neural Network that learns to predict the next character in a sequence. The RNN can then be used to generate text character by character that will look like the original training data.

Temperature:
An important parameter you may want to play with is -temperature, which takes a number in range (0, 1] (0 not included), default = 1. The temperature is dividing the predicted log probabilities before the Softmax, so lower temperature will cause the model to make more likely, but also more boring and conservative predictions. Higher temperatures cause the model to take more chances and increase diversity of results, but at a cost of more mistakes 

This code takes inspiration from Deeplearning.ai and Andrej Karpathy's blog-The Unreasonable Effectiveness of Recurrent Neural Networks.
