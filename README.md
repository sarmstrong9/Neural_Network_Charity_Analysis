# Neural_Network_Charity_Analysis



optimize step 1 - increase # of neurons to roughly triple the input layers to 120 and 60 respectively
optimize step 2 - remove "APPLICATION_TYPE" column from dataset as this seemed like fairly arbitrary data - adjust neurons to 105 and 53 resepctively based on new input dimensions
optimize step 3 - add back in "APPLICATION TYPE" since accuracy got worse from step 1, and then add a third hidden layer, increase neurons to 120 for all layers and increase epochs to 75

![Original Inputs](/results/original_model_inputs.png)
![Original Results](/results/original_model_results.png)
![Optimize 1 Inputs](/results/optimize_attempt1_increase_neurons_epochs.png)
![Optimize 1 Results](/results/optimize_attempt1_results.png)
![Optimize 2 Inputs](/results/optimize_attempt2_remove_application_type_column.png)
![Optimize 2 Results](/results/optimize_attempt2_results.png)
![Optimize 3 Inputs](/results/optimize_attempt3_add_hiddenlayer_increase_neurons.png)
![Optimize 3 Results](/results/optimize_attempt3_results.png)