- `VAESave`: The VAESave node is designed for saving VAE models along with their metadata, including prompts and additional PNG information, to a specified output directory. It encapsulates the functionality to serialize the model state and associated information into a file, facilitating the preservation and sharing of trained models.
    - Inputs:
        - `vae` (Required): The VAE model to be saved. This parameter is crucial as it represents the model whose state is to be serialized and stored. Type should be `VAE`.
        - `filename_prefix` (Required): A prefix for the filename under which the model and its metadata will be saved. This allows for organized storage and easy retrieval of models. Type should be `STRING`.
    - Outputs:
