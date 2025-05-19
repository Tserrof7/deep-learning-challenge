**Overview:** Explain the purpose of this analysis.
-----------------------------------------------------
The goal of the analysis here is to develop a machine learning model that can help a nonproit foundation
select applications for funding with the highest change of success.



                    ***Results***
-----------------------------------------------------
**Data Preprocessing**
-----------------------------------------------------
*What variable(s) are the target(s) for your model?*
-----------------------------------------------------
The target variable for this model is the "IS_SUCCESSFUL" column


*What variable(s) are the features for your model?*
-----------------------------------------------------
The features in this model are the following columns:
	
APPLICATION_TYPE	
AFFILIATION	
CLASSIFICATION
USE_CASE	
ORGANIZATION	
STATUS	
INCOME_AMT
ASK_AMT

*What variable(s) should be removed from the input data because they are neither targets nor features?*
-----------------------------------------------------
The two variables that needed to be removed were the following coumns:
EIN 
NAME


**Compiling, Training, and Evaluating the Model**
-----------------------------------------------------

*How many neurons, layers, and activation functions did you select for your neural network model, and why?*
-----------------------------------------------------
In the first verison of the machine learning model, it consisted of 1 input 1 and hidden layer, with an output layer. The first layer had 10 neurons and an activation fucnction of "relu". The second layer had 5 neurons, and also activation function of "relu". Output layer had 1 neuron, and an activation function "sigmoid".

Both second and third versions had 4 layers with 3 being hidden layers, both consecutively with 12, 6, 3, and 1 neurons in each layer.
However, while I kept the activation function in the second layer as "relu" in the third version, in the second version I decided to change the activation function to "tanh" to see if it would have a positive impact on performance.


*Were you able to achieve the target model performance?*
-----------------------------------------------------
I was not able to, the highest accuracy rating I was able to get was 73% in both version 2 and 3 of my optimization attempts.


*What steps did you take in your attempts to increase model performance?*
-----------------------------------------------------
* Changed amount of layers
* Changed amount of neurons in each layer
* Attempted to use a different activation function in a layer in one version
* Changed input dimensions


**Summary:**
 -----------------------------------------------------
Overall, through my attempts of trying to reach an accuracy score of 75% i was only able to reach 73%.
Both my second and third versions ended up using more neurons and layers than the first version, and were only slightly more accurate.
