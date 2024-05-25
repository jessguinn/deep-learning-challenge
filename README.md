# Neural Network Model Analysis

## Overview of the Analysis ##

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With a machine learning and neural networks from the provided dataset using binary classifier that can predict wheather applicants will be sucessful if funded by Alphabet Soup.

## Results ##

* Data Preprocessing
    * Target Variable: "IS_SSUCCESSFUL" is that main target variable for the model as it indicates if the organization has given funding to a charity that has been successful.
    * Featured Variables:
        - "APPLICATION_TYPE"
        - "AFFILIATION"
        - "CLASSIFICATION"
        -  "USE_CASE"
        -  "ORGANIZATION"
        -  "STATUS"
        -  "INCOME_AMT"
        -  "SPECIAL_CONSIDERATIONS"
        -  "ASK_AMT"
    * Removed Variables:
        - "EIN"
        - "NAME"

## Compiling, Training, and Evaluating the Model ##

  * 1st Attempt: The model used 18 neurons and 9 layers, using relu and sigmoid as the activation functions and 200 epochs. The accuracy result was 73.21% with a loss of 55.44%.
    
Model

![1st Attempt Alphabet Soup](https://github.com/jessguinn/deep-learning-challenge/assets/151950669/a38d7b8d-2f81-414d-aa6c-bbef6319e69b)

Accuracy and Loss

![1st Attempt Accuracy Alphabet Soup](https://github.com/jessguinn/deep-learning-challenge/assets/151950669/c95a0cf3-edfe-44c5-8267-d7926fc5373b)

   * Best Model Attempt: In this model the tuner was used to optimize performance. The model used 18 neurons and added second and third layers, using relu, tanh, and sigmoid as the activation functions and 20 epochs. The accuracy result was 92% with a loss of 18.53%. Achieving a higher accuracy result and lower loss result.
     
Tuner

![Best Model Tuner](https://github.com/jessguinn/deep-learning-challenge/assets/151950669/fd5f22ae-e68d-41f8-9d25-541c5408ac04)

Model

![Best Model Alphabet Soup](https://github.com/jessguinn/deep-learning-challenge/assets/151950669/f4b09ee2-f5a8-4b13-a874-56a3628b9fd8)

Accuracy and Loss

![Best Model Accuracy Alphabet Soup](https://github.com/jessguinn/deep-learning-challenge/assets/151950669/db09ca53-a6f3-4c98-99a0-96a8141ea6e1)

## Summary ##

The machine learning model achieved a higher performance with the tuner and changes to the model neurons, the final result of accuracy improved from 73.21% to 93% and reduction in loss from 55.44% to 18.53%. Additional activatition layers, and changing epochs drastically changed the final results to a cleaner and optimal prediction model.


