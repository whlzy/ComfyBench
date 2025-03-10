- `HypernetworkLoader (dirty)`: The HypernetworkLoader node is designed to enhance or modify the capabilities of a given model by applying a hypernetwork patch. This process involves loading a specified hypernetwork and applying it to the model with a certain strength, thereby potentially altering the model's behavior or performance based on the characteristics of the hypernetwork.
    - Inputs:
        - `model` (Required): The model to which the hypernetwork patch will be applied. This parameter is crucial as it determines the base model that will be enhanced or modified by the hypernetwork. Type should be `MODEL`.
        - `hypernetwork_name` (Required): The name of the hypernetwork to be loaded and applied. This parameter specifies which hypernetwork patch will be used to modify the model. Type should be `STRING`.
        - `strength` (Required): The strength with which the hypernetwork patch will be applied to the model. This affects the intensity of the modification or enhancement. Type should be `FLOAT`.
    - Outputs:
        - `model`: The modified model after the hypernetwork patch has been applied. This output reflects the changes made to the original model by the hypernetwork. Type should be `MODEL`.
