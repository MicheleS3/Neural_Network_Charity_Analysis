# Neural_Network_Charity_Analysis

### Overview

With our knowledge of machine learning and neural networks, we’ll use the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.  From Alphabet Soup’s business team, we received a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.  Using our knowledge of TensorFlow, optimize the model in order to achieve a target predictive accuracy higher than 75%. 

### Results

•	Data Preprocessing

    oThe data provided shows a column for 'IS_SUCCESSFUL,' and will be the targeted data point for these predictions.

    oThere are many data points (features) that will be used as input for the models. Included are:

    - AFFILIATION
    - APPLICATION_TYPE
    - ASK_AMT
    - CLASSIFICATION
    - INCOME_AMT
    - ORGANIZATION
    - SPECIAL_CONSIDERATIONS
    - STATUS
    - USE_CASE
    
    oThe columns for "NAME" and "EIN" have no direct effect on the success/falure rate, and have been excluded from processing.

•	Compiling, Training, and Evaluating the Model

  - Original Model - Layer 1 = 80 Activation = Relu
                   - Layer 2 = 30  Activation = Relu
  
  - 1st Attempt    - Layer 1 = 120 Activation = Relu
                   - Layer 2 = 90  Activation = Relu

  - 2nd Attempt    - Layer 1 = 150 Activation = Relu
                   - Layer 2 = 70  Activation = Relu
                   - Layer 3 = 50  Activation = Relu

  - 3rd Attempt    - Layer 1 = 250 Activation = Sigmoid
                   - Layer 2 = 150 Activation = Sigmoid
                   - Layer 3 = 60  Activation = Sigmoid

### Summary

The initial model had an accuracy of 52.9% of success when Alphabet Soup invested with an organization.

![1st Attempt results](https://user-images.githubusercontent.com/89753083/158234379-814fb0c0-25a6-4dad-9a49-bc83d1b1c7ff.PNG)

Below are the additional 3 attempts to improve prediction accuracy.

![Deliverable 3 1st attempt results](https://user-images.githubusercontent.com/89753083/158234530-dd6d9e58-faf9-4acb-9a6b-5d47610d03d5.PNG)

![Deliverable 3 2nd attempt results](https://user-images.githubusercontent.com/89753083/158234545-6852b6ea-bc91-492d-93ce-a5cba7c161fa.PNG)

![Deliverable 3 3rd attempt results](https://user-images.githubusercontent.com/89753083/158234565-4522ea33-5c8f-459a-b533-80c82f669e78.PNG)

To further investigate these tests we recommend alternative, non-sequential hyperparameter models. Another means of improving accuracy is to have more datapoints. Although we did not boost success rate to 75%, we have minimized loss using these tuned models.
