# Neural_Network_Charity_Analysis
## Overview of the analysis:
- The purpose of this analysis was to understand the benefits and challenges of designing and implementing a more complicated machine learning model with neural networks.

## Results:

### Data Preprocessing
- For this particular model, the target variables were: Application Type, Affiliation, Classfication, Use Case, Organziation, Status, Income Amount, Special Considerations, Ask Amount
- The feature variable for this model was 'Is Successful'
- The variables that were removed from the model were EIN and Name. These had no particular value to the model and would only cause more 'noise' for the model

### Compiling, Training, and Evaluating the Model
- In the first model, there were 2 hidden layers with 80 layers for the 1st, and then 30 for the second. The activation for the 1st and 2nd layers were 'relu' method and the output layer was 'sigmoid'.
- I did not achieve the 75% threshold for success. I achieved 73% with my original challenge script, and then 72% with my 2nd optimized attempt
- I took a variety of steps to try and optimize the model. In my first attempt, i tried to remove additional columns (e.g., Affiliation) which dropped my performance to less than 65%. In the 2nd attempt, i increased the number of hidden nodes and kept the activation as a relu. That ultimately achieved 72%. In the 3rd attempt, I dropped more columns and increased the number of EPOCHs. This had the inverse effect on the outcomes. It dropped to 63%

### Summary: 
In summary, the largest impact on the model appeared to relate more to the activation and adding of additional layers. From my understanding of the module, the more layers of a neural networking model, the stronger it can be. I think I missed out on changing the activation type as i kept my similar throughout. As far as what i would do different, i think i would leverage a logistic regression model or a random forest.
