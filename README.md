# Neural Network Charity Analysis
## Purpose
The purpose of this project is to lend our skill to a foundation in order to help them know where to place their investments. The goal is to use machine learning and neural networks to determine if applicants will be successful so the foundation can better manage where they are investing their money. 

## Results
### Data Preprocessing
- Feature variables include all columns except for the target and the varaibles that were dropped (listed below)
- Target variables is the IS_SUCCESSFUL column
- Variables that were removed from the dataset:  EIN and NAME columns were removed originally.  As part of the optimization process, the STATUS column was also removed.

### Compiling, Training, and Evaluating the Model
- Initially, the model started with two hidden layers with 80 and 30 neurons respectively both of which had the relu activation. The model ran with 40 epochs and reach an accuracy of 55.7%
- Though multiple attempts were tried, I did not reach the 75% accuracy level.  
- As part of the optimization process, I increased the epochs to 30 and the hidden layer 1 neurons to 100 and hidden layer 2 neurons to 90.  I increased the neurons becuase it can help the model's predicitive power and then I added epochs to accommodate the added compelxity. 
<img width="656" alt="Attempt 1" src="https://user-images.githubusercontent.com/85457256/137414896-91bb7c0b-aec5-4910-a8f6-5dc71eca4eca.png">


- For the second attempt I tried increasing the number of epochs to 100 to see if the model reached another point where it could increase its performance. I also removed the STATUS column as I wondered if it could be misleading the model. 
<img width="641" alt="Attempt 2" src="https://user-images.githubusercontent.com/85457256/137415037-e006392c-516e-4bca-a66b-e6cd6b2ff65c.png">


- As the previous two attempts did not yeild desired results,I kept the first attempt parameters but also added a third hidden layer with 70 neurons and a relu activation. I chose this as adding more hidden layers can help the model improve performance.  As the results show, though, this actually produced a much lower accuracy level.
<img width="693" alt="Attempt 2" src="https://user-images.githubusercontent.com/85457256/137413043-3b68fac7-0be5-4a4e-a77a-cd52fa5b9f16.png">


## Summary
Overall, the desired accuracy was not achieved as the highest accuracy was achieved in attempt 2 at 69.8%.  An alternative model to use is a Random Forest model as it can also classify datasets into various outputs.  This type of model handles tabular data which is the data in the dataset and in order to be successful would need multiple layers so it can be trained properly and produce a high level of accuracy.  

