# deep-learning-challenge
Overview of the Analysis
The analysis was conducted to develop a deep learning model capable of predicting the success of philanthropic efforts by Alphabet Soup based on certain variables. As Alphabet Soup receives numerous applications for funding from various projects, the aim was to classify which projects are more likely to succeed or fail, to distribute resources more effectively.
________________________________________
Results
Data Preprocessing
•	What variable(s) are the target(s) for your model?
o	The target variable for this model is the "Success" of the project, which may be categorized as "Successful" or "Unsuccessful."
•	What variable(s) are the features for your model?
o	The feature variables are taken from application_df and were defined by dropping the 'IS_SUCCESSFUL' column from the original data frame.
•	What variable(s) should be removed from the input data because they are neither targets nor features?
o	Both 'EIN' and 'NAME' columns were dropped because they had no relevance to the features for the dataset.
Compiling, Training, and Evaluating the Model
•	How many neurons, layers, and activation functions did you select for your neural network model, and why?
o	The neural network consists of 3 layers. The first layer has 80 neurons, the second layer has 30, and the third layer has 10. The activation functions used were ReLU for the input and hidden layers and sigmoid for the output layer. The rationale behind this design was to capture the complexity of the input data and provide a refined output.
•	Were you able to achieve the target model performance?
o	No, the model achieved an accuracy rate of 74% which was below the desired threshold of 75%.
•	What steps did you take in your attempts to increase model performance?
o	Implemented feature scaling using MinMaxScaler.
o	Tweaked the number of neurons and layers in the neural network.
o	Experimented with different activation functions.
o	Used dropout layers to prevent overfitting.
o	Adjusted the batch size and number of epochs during training.
________________________________________
Summary
The deep learning model developed for Alphabet Soup's philanthropic project classification performed just below satisfactorily, despite numerous tweaks, achieving a model accuracy of 74%. This model will aid Alphabet Soup in making informed decisions about which projects to fund, ensuring optimal utilization of resources.
Recommendation: For further enhancement in model performance or to tackle the problem from a different perspective, further exploration online provided information that an ensemble method such as Random Forest can be explored. This algorithm is known for its high accuracy and ability to handle large datasets. It can capture non-linear patterns and often requires less preprocessing. Additionally, these models can give insight into feature importance, which can be invaluable for understanding which variables most significantly impact project success.
