# Soft Computing

# Requirement :

**Install Python3**

*For Ubuntu* :
```bash
	sudo apt install python3 python3-pip
```

This repository contains the python implementation for a few soft computing algorithms.

Implemented algorithms:

- Hebb Net
- Single layer perceptron
- Multi layer perceptron (single hidden layer)
- BAM
- Fuzzy
- Hamming
- Kohenen
- McCullochPitt
- MaxNet

### Cloning the repository

Clone the repository using:

```bash
  git clone https://github.com/SUGAM-ARORA/Soft-Computing.git

Move into the cloned repository:

```bash
  cd Soft-Computing
```

Install the required dependencies:

```bash
  pip install -r requirements.txt
```

### Usage/Examples

Import the packages from different modules using:

```python
from hebbnet.hebb_net import HebbNet
from single_layer_perceptron.slp import SingleLayerPerceptron
```

Create the model for each algorithm using:

```python
input_list = [[1, 1], [1, -1], [-1, 1], [-1, -1]]
targets = [1, -1, -1, -1]

hebb_model = HebbNet()
slp_model = SingleLayerPerceptron()

hebb_model.train_model(input_list, targets)
slp_model.train_model(input_list, targets, alpha=1, max_epochs=3)
```