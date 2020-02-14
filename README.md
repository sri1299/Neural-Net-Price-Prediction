# Neural-Net-Price-Prediction
## Dataset
Diamond dataset from Kaggle(https://www.kaggle.com/shivam2503/diamonds) was used to predict prices using Neural Network Regression.
The dataset contains:
price price in US dollars (\$326--\$18,823)
carat weight of the diamond (0.2--5.01)
cut quality of the cut (Fair, Good, Very Good, Premium, Ideal)
color diamond colour, from J (worst) to D (best)
clarity a measurement of how clear the diamond is (I1 (worst), SI2, SI1, VS2, VS1, VVS2, VVS1, IF (best))
x length in mm (0--10.74)
y width in mm (0--58.9)
z depth in mm (0--31.8)
depth total depth percentage = z / mean(x, y) = 2 * z / (x + y) (43--79)
The column with string entry was changed into one-hot encoded columns based number of unique entries.
## Neural Network
Package used: PyTorch
A simple Feed Forward Neural Network (3-hidden layers) was used. 
Activation Function: LeakyReLU
Xavier initialisation is used to initialise the weights.
Data was sent in mini-batches of 128.
Convergence is easily achieved after few thousands of epochs.
## Results
Training Accuracy: 98.21%
Test Accuracy: 98.06%
