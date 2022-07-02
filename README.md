# Neural_Network_Charity_Analysis



optimize step 1 - increase # of neurons to roughly triple the input layers to 120 and 60 respectively
optimize step 2 - remove "APPLICATION_TYPE" column from dataset as this seemed like fairly arbitrary data - adjust neurons to 105 and 53 resepctively based on new input dimensions
optimize step 3 - add back in "APPLICATION TYPE" since accuracy got worse from step 1, and then add a third hidden layer, increase neurons to 120 for all layers and increase epochs to 75

- Original Model
    - Inputs
        - ![Original Inputs](results/original_model_inputs.png)
    - Results
        - ![Original Results](results/original_model_results.png)
- Optimization Attempt 1
    - Inputs
        - ![Optimize 1 Inputs](results/optimize_attempt1_increase_neurons_epochs.png)
    - Results
        - ![Optimize 1 Results](results/optimize_attempt1_results.png)
- Optimization Attempt 2
    - Inputs
        - ![Optimize 2 Inputs](results/optimize_attempt2_remove_application_type_column.png)
    - Results
        - ![Optimize 2 Results](results/optimize_attempt2_results.png)
- Optimization Attempt 3
    - Inputs
        - ![Optimize 3 Inputs](results/optimize_attempt3_add_hiddenlayer_increase_neurons.png)
    - Results
        - ![Optimize 3 Results](results/optimize_attempt3_results.png)