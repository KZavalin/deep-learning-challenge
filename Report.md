Report of Predicting Venture Success Chance by a Neural Network Model for Alphabet Soup Charity 

OVERVIEW

    The purpose of this analysis was to create a model for predicting venture success chance of applicants for funding by the nonprofit foundation Alphabet Soup. This model used trained and tested on an existing database of previous applicants whose venture success chance is known. 

RESULTS

    *Data Preprocessing

        -Target of this model was predicting whether the venture was successful ('IS SUCCESSFUL' in the dataframe).
    
        -Variables used as features include: application type, affiliated sector of industry, government organization classification, use case for funding, organization type, whether the venture status is active, income classification, special considerations for application, and the funding amount requested. 
    
        -Identification columns (EIN and NAME) were neither targets nor features, and were excluded from modeling.

    *Compiling, Training, and Evaluating the Model

        -This neural network model used three hidden layers of 80, 50, and 50 neurons (units), respectively, using a relu activation function; the output layer contained one neuron using the sigmoid activation function. Different activation functions (leaky relu, linear, tahn), additional hidden layers, numbers of neurons, and training epochs were also tried, but they did not significantly increase the model accuracy nor decrease the model loss. 

    *Were you able to achieve the target model performance?
        -Unfortunately, the many permutations of neurons, layers, training epochs, and activation functions consistently yielded the same approximate results of 72-73% model accuracy. Sometimes, overtraining was possible, but the accuracy would still be around this amount when evaluating with the test dataset. Likely, this reflects the inherent stochastic property of the data or presence of influencial features that are not present in this dataset and not available for making this model.


    *What steps did you take in your attempts to increase model performance?
        -To increase model performance, the following parameters were tried: different neuron numbers (10-80 units), different number of hidden layers (2-8 layers), different activation functions (leaky relu, relu, linear, tahn), and different number of epochs (100-1000).

SUMMARY

In this exercise, a neural network model was created for predicting venture success chance of applicants for funding by the nonprofit foundation Alphabet Soup. While multiple parameter settings were attempted for this model, its predictive value still comes with an accuracy of ~72% and loss of .57. These reflect a low accuracy, and this model should be further improved if it is to serve as a predictive tool. Most likely, an expanded dataset that includes more cases and an increased number of features would be of benefit in creating a better model. Another model that could solve this classification problem would be a logistic regression model, which is optimized for predicting binary outcomes such as success or failure of a venture in this case.


