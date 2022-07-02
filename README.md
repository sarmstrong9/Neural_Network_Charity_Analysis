# Neural_Network_Charity_Analysis

## **Overview**:
Explain the purpose of this analysis.


Using machine learning and neural networks and the features in the provided dataset, create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

The analysis will be accomplished utilizing a CSV obtained From Alphabet Soup’s business team containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

**EIN** and **NAME** — Identification columns  
**APPLICATION_TYPE** — Alphabet Soup application type  
**AFFILIATION** — Affiliated sector of industry  
**CLASSIFICATION** — Government organization classification  
**USE_CASE** — Use case for funding  
**ORGANIZATION** — Organization type  
**STATUS** — Active status  
**INCOME_AMT** — Income classification  
**SPECIAL_CONSIDERATIONS** — Special consideration for application  
**ASK_AMT** — Funding amount requested  
**IS_SUCCESSFUL** — Was the money used effectively  

  
## **Results**: 
The results from this analysis help to address the following questions:

- Data Preprocessing  
    - What variable(s) are considered the target(s) for your model?  
        - The "IS_SUCCESSFUL" column is the target column as this is the result of what determined if the campaign was successful or not.
    - What variable(s) are considered to be the features for your model?  
        - All columns except the "IS_SUCCESSFUL" are features of the model, except the "EIN" and "NAME" columns.
    - What variable(s) are neither targets nor features, and should be removed from the input data?  
        - The "EIN" and "NAME" columns
- Compiling, Training, and Evaluating the Model  
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?  
        - After completing all the optimization steps, the model used 3 hidden layers, each with 120 neurons.  The "relu" activation function was utilized with 75 epochs.  These were chosen because bumping up the quantity of neurons and hidden layers had achieved the goal of improving model accuracy in prior models.  I continued using the "relu"activation layer as this is what the original model was based off as well.
    - Were you able to achieve the target model performance?
        - I was not able to achieve target model performance of 75% or greater.
    - What steps did you take to try and increase model performance?  
        - Optimize Step 1 - I increased the number of neurons to roughly triple the input layers to 120 and 60 respectively  
        - Optimize Step 2 - I removed the "APPLICATION_TYPE" column from dataset as this seemed like fairly arbitrary data.  I also adjusted the neurons to 105 and 53 respectively based on new input dimensions.  
        - Optimize Step 3 - I added back in "APPLICATION TYPE" column since accuracy got worse compared to step 1, and then added a third hidden layer and increased neurons to 120 for all layers and increase epochs to 75.  

## **Summary**: 
The overall results of the deep learning model are shown below, including the initial model and the three attempts to optimize the results.  

- Original Model
    - Inputs
        ![Original Inputs](results/original_model_inputs.png)  
    - Results  
            ![Original Results](results/original_model_results.png)
- Optimization Attempt 1
    - Inputs  
        ![Optimize 1 Inputs](results/optimize_attempt1_increase_neurons_epochs.png)
    - Results  
        ![Optimize 1 Results](results/optimize_attempt1_results.png)  
- Optimization Attempt 2
    - Inputs  
        ![Optimize 2 Inputs](results/optimize_attempt2_remove_application_type_column.png)
    - Results  
        ![Optimize 2 Results](results/optimize_attempt2_results.png)
- Optimization Attempt 3
    - Inputs  
        ![Optimize 3 Inputs](results/optimize_attempt3_add_hiddenlayer_increase_neurons.png)
    - Results  
        ![Optimize 3 Results](results/optimize_attempt3_results.png)  


A recommendation for how a different model could solve this classification problem could be to use the "RandomForest" model.  This model has proven to be very effective with classification problems in the past, and since the neural network model was having trouble bumping up the accuracy I would recommend trying this model instead.  
