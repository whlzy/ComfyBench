- `LoRA Stacker`: The LoRA Stacker node is designed to aggregate and configure LoRA (Low-Rank Adaptation) parameters into a structured format, facilitating the manipulation and application of LoRA adjustments across different model components. It supports dynamic configuration through input parameters, allowing for the customization of LoRA parameters based on specific requirements.
    - Inputs:
        - `input_mode` (Required): Specifies the mode of input processing, determining how LoRA parameters are aggregated and structured. It affects the configuration and representation of LoRA parameters in the output. Type should be `COMBO[STRING]`.
        - `lora_count` (Required): Defines the number of LoRA adjustments to be considered, dictating the scale of aggregation and the number of parameters to be processed. Type should be `INT`.
        - `lora_name_i` (Required): Specifies the name of each LoRA parameter, allowing for the identification and configuration of individual LoRA adjustments. Type should be `COMBO[STRING]`.
        - `lora_wt_i` (Required): Determines the weight of each LoRA parameter, influencing the impact of the adjustment on the model. Type should be `FLOAT`.
        - `model_str_i` (Required): Specifies the strength of the model adjustment for each LoRA parameter, affecting the model's behavior. Type should be `FLOAT`.
        - `clip_str_i` (Required): Defines the clipping strength for each LoRA parameter, controlling the extent of adjustment applied. Type should be `FLOAT`.
        - `lora_stack` (Optional): An optional stack of pre-configured LoRA parameters that can be extended or modified with the current configuration, enhancing flexibility in LoRA parameter management. Type should be `LORA_STACK`.
    - Outputs:
        - `LORA_STACK`: Returns a structured representation of LoRA parameters, ready for further processing or application within model components. Type should be `LORA_STACK`.
