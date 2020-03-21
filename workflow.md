## My deep learning workflow

# step 1: package selection

- Import all the packages into one cell of the Notebook (packages for data cleaning, model development and evaluation)

# step 2: Settings

- device configuration (pytorch)
- hyperparameters definitions (deep learning)
- load the data and explore

# step 3: Define the arcitecture of the model such as

- Define the init method

  - The number of hidden units in the input layers; which is determined by the features of the data
  - Number of total hidden layers in the model (iterative)
  - Number of hidden units in each hidden layers (iterative)
  - The output layer node units is determined by the intended outcome to achieve

- Define the forward method
  - make predictions

# step 4: Loss and optimizer definition

- Instantiate the model class
- Select a loss metrics
- Select an optimizer, preferably “Adam”

# step 5: Training process

- Iterate through the data
- Forward prop (making prediction i.e summation of all the layers (weight matrices and bias vector with their activation functions to compute the prediction)
- Compute the cost function J (difference in the real output and the predicted output
- Back prop to compute the gradient wrt J (objective function)
- Updates the model parameters [weights and bias] (optimizer step)

# step 6: Evaluation

- print the metrics