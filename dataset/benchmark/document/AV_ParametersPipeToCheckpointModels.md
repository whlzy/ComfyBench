- `AV_ParametersPipeToCheckpointModels`: This node is designed to transform a set of parameters encapsulated within a pipe structure into specific model checkpoint names and configurations. It serves as a bridge between abstract parameter definitions and concrete model instantiation, facilitating the dynamic selection and configuration of models based on provided parameters.
    - Inputs:
        - `pipe` (Required): The pipe parameter acts as a container for model-related parameters, including checkpoint names, VAE names, and upscaler names. It plays a crucial role in determining the specific models and configurations to be instantiated based on the encapsulated parameters. Type should be `PIPE`.
    - Outputs:
        - `pipe`: Returns the updated pipe structure, now including the resolved names and configurations for model checkpoints, VAEs, and upscalers, based on the input parameters. Type should be `PIPE`.
        - `ckpt_name`: The primary checkpoint model name derived from the input parameters. Type should be `CHECKPOINT_NAME`.
        - `secondary_ckpt_name`: The secondary checkpoint model name derived from the input parameters. Type should be `CHECKPOINT_NAME`.
        - `vae_name`: The name of the VAE model derived from the input parameters. Type should be `VAE_NAME`.
        - `upscaler_name`: The name of the primary upscaler model derived from the input parameters. Type should be `UPSCALER_NAME`.
        - `secondary_upscaler_name`: The name of the secondary upscaler model derived from the input parameters. Type should be `UPSCALER_NAME`.
        - `lora_1_name`: The name of the first Lora model derived from the input parameters. Type should be `LORA_NAME`.
        - `lora_2_name`: The name of the second Lora model derived from the input parameters. Type should be `LORA_NAME`.
        - `lora_3_name`: The name of the third Lora model derived from the input parameters. Type should be `LORA_NAME`.
