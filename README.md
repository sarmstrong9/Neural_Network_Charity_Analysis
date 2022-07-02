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
        - asdf
    - What variable(s) are considered to be the features for your model?  
        -asdf 
    - What variable(s) are neither targets nor features, and should be removed from the input data?  
        - asdf
- Compiling, Training, and Evaluating the Model  
    - How many neurons, layers, and activation functions did you select for your neural network model, and why?  
        - asdf  
    - Were you able to achieve the target model performance?
        - asdf  
    - What steps did you take to try and increase model performance?  
        - asdf



optimize step 1 - increase # of neurons to roughly triple the input layers to 120 and 60 respectively
optimize step 2 - remove "APPLICATION_TYPE" column from dataset as this seemed like fairly arbitrary data - adjust neurons to 105 and 53 resepctively based on new input dimensions
optimize step 3 - add back in "APPLICATION TYPE" since accuracy got worse from step 1, and then add a third hidden layer, increase neurons to 120 for all layers and increase epochs to 75

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


## **Summary**: 
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.