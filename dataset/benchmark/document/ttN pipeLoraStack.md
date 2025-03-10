- `ttN pipeLoraStack`: The node is designed to integrate and manage LoRA (Low-Rank Adaptation) models within a processing pipeline, enabling the dynamic adjustment of model and clip strengths based on specified LoRA configurations. It facilitates the customization of AI model behavior for specific tasks or datasets by applying LoRA modifications to the underlying models.
    - Inputs:
        - `toggle` (Required): A boolean toggle to enable or disable the application of LoRA models within the pipeline. Type should be `COMBO[BOOLEAN]`.
        - `mode` (Required): Specifies the operation mode, either 'simple' or 'advanced', determining the complexity of LoRA model adjustments. Type should be `COMBO[STRING]`.
        - `num_loras` (Required): The number of LoRA models to be applied, allowing for multiple adaptations. Type should be `INT`.
        - `optional_pipe` (Optional): An optional pipeline configuration that can be modified by the LoRA adjustments. Type should be `PIPE_LINE`.
        - `model_override` (Optional): Allows for overriding the default model with a specified one for further customization. Type should be `MODEL`.
        - `clip_override` (Optional): Enables the override of the default clip model, facilitating custom clip adaptations. Type should be `CLIP`.
        - `optional_lora_stack` (Optional): A stack of LoRA models that can be optionally applied for layered adaptations. Type should be `LORA_STACK`.
        - `lora_i_name` (Optional): Specifies the name of the ith LoRA model to be applied, determining the specific adaptation for each model. Type should be `COMBO[STRING]`.
        - `lora_i_strength` (Optional): Defines the strength of the ith LoRA model adaptation, influencing the degree of modification. Type should be `FLOAT`.
        - `lora_i_model_strength` (Optional): Determines the model-specific strength of the ith LoRA adaptation, affecting the model's behavior. Type should be `FLOAT`.
        - `lora_i_clip_strength` (Optional): Specifies the clip-specific strength of the ith LoRA adaptation, modifying the clip's influence. Type should be `FLOAT`.
    - Outputs:
        - `optional_pipe`: The modified pipeline configuration after applying LoRA adjustments, including any model or clip overrides. Type should be `PIPE_LINE`.
        - `lora_stack`: A stack of LoRA models that have been applied, detailing each model's name and its model and clip strengths. Type should be `LORA_STACK`.
