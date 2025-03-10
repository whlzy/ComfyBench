- `SeargeOutput5`: SeargeOutput5 is designed to demultiplex and output prompt processing parameters, including various scales and powers related to base and refiner conditioning, as well as style prompt power adjustments. This node plays a crucial role in fine-tuning the generation process by providing detailed control over the influence of different components on the final output.
    - Inputs:
        - `parameters` (Required): The 'parameters' input contains key-value pairs specifying the scales and powers for base conditioning, refiner conditioning, style prompt, and negative style, which are essential for adjusting the generation process. Type should be `PARAMETERS`.
    - Outputs:
        - `parameters`: Returns the original set of parameters provided as input, allowing for further processing or utilization downstream. Type should be `PARAMETERS`.
        - `base_conditioning_scale`: Specifies the scale factor for base conditioning, influencing the initial stage of generation. Type should be `FLOAT`.
        - `refiner_conditioning_scale`: Determines the scale factor for refiner conditioning, affecting the refinement stage of generation. Type should be `FLOAT`.
        - `style_prompt_power`: Indicates the power applied to the style prompt, adjusting its influence on the generation. Type should be `FLOAT`.
        - `negative_style_power`: Specifies the power applied to negative styles, allowing for the reduction of unwanted stylistic elements. Type should be `FLOAT`.
