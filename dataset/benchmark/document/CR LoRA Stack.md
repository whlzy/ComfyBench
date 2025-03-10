- `CR LoRA Stack`: The CR LoRA Stack node is designed to create and manage a stack of LoRA (Low-Rank Adaptation) modifications for models. It allows for the sequential application of multiple LoRA modifications to a model, enabling fine-tuned adjustments to model behavior and performance.
    - Inputs:
        - `switch_1` (Required): Controls whether the first LoRA modification is applied. This switch enables selective application of modifications. Type should be `COMBO[STRING]`.
        - `lora_name_1` (Required): Specifies the first LoRA modification to be applied. It is crucial for defining the initial step in the sequence of LoRA adjustments. Type should be `COMBO[STRING]`.
        - `model_weight_1` (Required): Determines the weight of the first LoRA modification on the model. This weight influences the extent of the modification's impact. Type should be `FLOAT`.
        - `clip_weight_1` (Required): Sets the weight of the first LoRA modification on the clip. This weight affects how significantly the clip is modified. Type should be `FLOAT`.
        - `switch_2` (Required): Controls the application of the second LoRA modification, offering more granular control over the adjustments. Type should be `COMBO[STRING]`.
        - `lora_name_2` (Required): Specifies the second LoRA modification in the sequence. It allows for further customization following the initial modification. Type should be `COMBO[STRING]`.
        - `model_weight_2` (Required): Determines the weight of the second LoRA modification on the model, further adjusting its behavior. Type should be `FLOAT`.
        - `clip_weight_2` (Required): Sets the weight of the second LoRA modification on the clip, modifying its characteristics further. Type should be `FLOAT`.
        - `switch_3` (Required): Enables or disables the third LoRA modification, providing ultimate control over the stack. Type should be `COMBO[STRING]`.
        - `lora_name_3` (Required): Defines the third LoRA modification in the stack, extending the customization capabilities. Type should be `COMBO[STRING]`.
        - `model_weight_3` (Required): Specifies the weight of the third LoRA modification on the model, allowing for additional fine-tuning. Type should be `FLOAT`.
        - `clip_weight_3` (Required): Determines the weight of the third LoRA modification on the clip, further influencing its output. Type should be `FLOAT`.
        - `lora_stack` (Optional): Allows for the inclusion of an existing LoRA stack to be extended with new modifications. This parameter facilitates the building of complex LoRA sequences. Type should be `LORA_STACK`.
    - Outputs:
        - `LORA_STACK`: Returns the compiled list of LoRA modifications, ready for application to a model and clip. Type should be `LORA_STACK`.
        - `show_help`: Provides a URL to documentation or help related to the LoRA stack node, assisting users in understanding its use. Type should be `STRING`.
