# Neural State Classification
Neural network approach to the state classification problem implemented with Keras.

## 'models'
The 'models' directory contains two projects: 'helicopter_models', 'parametric_neuron_models'.

### 'helicopter_models'
'helicopter_models/networks.ipynb' implements a 1D CNN trained on 1 million example configurations from a hybrid automata model of a helicopter control system.

CNN Architecture:
16 3x1 convolutions => 32 3x16 convolutions => FC 2048 => FC 1024 => FC 512 => FC1

Dropout is applied in all fully connected layers except the output layer.  Batch normalization is applied to both convolutional and fully connected layers.

Accuracy: 95.6%

### 'parametric_neuron_models'
'parametric_neuron_models/networks.ipynb' contains 5 models trained on samples from a parametrized neuron model where the number of parameters varied between 1 and 5.

Accuracy: 97-99%
