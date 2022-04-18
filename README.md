# Neural_Network_Charity_Analysis

# Neural Networks and Deep Learning Models

## Overview of Project

### Purpose

The purpose of this to help Beks predict the success of an applicant if funded by her company. We will need to clean the data that her company uses to fit the model that we are going to use. We are using tensorflow keras library to make a neural network model to try to predict the outcome. Tensor flow uses hidden layers with neurons in them to analyze and predict the outcome of the data.

## Results

- Data Preprocessing
  - What variable(s) are considered the target(s) for your model?

The variables that I am using as the target for this model is the column 'IS_SUCCESSFUL'. Is column shows the result of the charity. I was able to get this data using the code below.

![image](https://user-images.githubusercontent.com/92827264/163736084-8e3a7046-9980-482c-a8ff-7e2fd40a6ae9.png)

  - What variable(s) are considered to be the features for your model?

The variables that I am using as the features are the rest of the dataset except for the columns: EIN, NAME, and IS_SUCCESSFUL. I created the features by using the code below.

![image](https://user-images.githubusercontent.com/92827264/163736230-13c2eedf-d406-4264-bb8c-394ded0d1652.png)

  - What variable(s) are neither targets nor features, and should be removed from the input data? 

The variables that are neither tagrets or features are 'EIN' and 'NAME' columns. I dropped these columns early on using the following code.

![image](https://user-images.githubusercontent.com/92827264/163736286-b7413f71-ee48-4f20-83b8-4c6786c44b64.png)

- Compiling, Training, and Evaluating the Model

  - How many neurons, layers, and activation functions did you select for your neural network model, and why?

I used a total of 110 neurons with 2 hidden layers. 80 neurons for hidden layer 1 and 30 neurons for hidden layer 2. The activation functions I am using are relu and sigmoid. I am using relu for my hidden layers and sigmoid for the output layer. I am using these parameters for my neural network becuase it is what the example wanted us to follow. A higher number of neurons for the hidden layers will give the model better accuracy which is why they choose 80 for layer one and 30 for layer 2. You can see my code for the parameters below.

![image](https://user-images.githubusercontent.com/92827264/163746861-cff35753-32a8-43a3-bdf9-d9c973aa47e3.png)
![image](https://user-images.githubusercontent.com/92827264/163746895-c6fdd6c8-0c5c-4a4d-86bc-b6c4756d2568.png)

  - Were you able to achieve the target model performance?

I was not able to achive a 75% accuracy for my model. After doing optimization it was still about 72% accuracy.

![image](https://user-images.githubusercontent.com/92827264/163747352-25df1e9b-f386-44e1-a705-1715cd57ea4a.png)


  - What steps did you take to try and increase model performance?

I tried increasing the number of neurons in my hidden layers, adding a third hidden layer, and increasing the number of epochs for the training.

![image](https://user-images.githubusercontent.com/92827264/163747330-42e36f8e-0332-475f-9f1d-8a5a44aac3d2.png)


## Summary

In summary the model preformed pretty well. It has aabout a 73% accuracy rate which is pretty high. I would of idealy like to make this better but I think with the type of data it is we would have to use a different model to get better accuracy. The model that I would use on this kind of data would be a supervised machine learning model like random forest. I think it would work better because we know what the is for our data set so it would be easier to use a supervised ML model.
