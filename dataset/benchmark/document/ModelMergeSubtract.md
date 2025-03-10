- `ModelMergeSubtract`: This node is designed for advanced model merging operations, specifically to subtract the parameters of one model from another based on a specified multiplier. It enables the customization of model behaviors by adjusting the influence of one model's parameters over another, facilitating the creation of new, hybrid models.
    - Inputs:
        - `model1` (Required): The base model from which parameters will be subtracted. Type should be `MODEL`.
        - `model2` (Required): The model whose parameters will be subtracted from the base model. Type should be `MODEL`.
        - `multiplier` (Required): A floating-point value that scales the subtraction effect on the base model's parameters. Type should be `FLOAT`.
    - Outputs:
        - `model`: The resulting model after subtracting the parameters of one model from another, scaled by the multiplier. Type should be `MODEL`.
