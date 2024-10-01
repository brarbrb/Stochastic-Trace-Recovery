# Sequence Probability Model Implementation
Final project in course - business process management and mining
based on Sequence Probability mapping from papper SKTR: Trace Recovery from Stochastically Known Logs
performed on BPI Challenge 2012 dataset   https://data.4tu.nl/articles/dataset/BPI_Challenge_2012/12689204

The main goal is to recover the true events in the log with some errors/noise (stochastic log). We've implemented similiar approach as in Section 3C in the paper mentioned. 

The steps we've implemented in this project are:
1. Splitting the data(deterministic logs) into train and test set
2. Creating noisy test logs with different noise levels - this step meant to mimic Stochastic log
3. Calculating transition probabilities based on the training data (deterministic) 
4. Implementing the Sequence Probability Model 
5. Evaluate the models' accuracies for different noise levels and sequence lengths using accuracy measure 



# Files
- `SKTR.ipynb`: The main Jupyter notebook containing the implementation.

  # Python Libraries used

- pm4py
- numpy
- matplotlib
- sklearn
- collections
- random


## Results

The notebook produces two key graphs:
1. **Model Accuracy vs Pa Values**: Shows the accuracy of the models for different noise levels.
2. **Model Accuracy vs Sequence Length**: Compares the accuracies of the SKTR model with different sequence lengths
