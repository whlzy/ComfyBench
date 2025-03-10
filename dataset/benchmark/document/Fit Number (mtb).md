- `Fit Number (mtb)`: The Fit Number node is designed to adjust a single numerical value to fit within a specified target range. It supports clamping to ensure the value stays within the target range and allows for the application of easing functions to modify the distribution of the transformed value.
    - Inputs:
        - `value` (Required): A single numerical value to be transformed. The node adjusts this value to fit within the specified target range, potentially altering its distribution based on the easing function applied. Type should be `FLOAT`.
        - `clamp` (Required): A boolean indicating whether to clamp the transformed value to the target range, ensuring it does not fall outside the specified limits. Type should be `BOOLEAN`.
        - `source_min` (Required): The minimum value of the source range. It is used as the lower bound when transforming the value. Type should be `FLOAT`.
        - `source_max` (Required): The maximum value of the source range. It serves as the upper bound for the transformation of the value. Type should be `FLOAT`.
        - `target_min` (Required): The minimum value of the target range. This is the lower limit to which the input value is scaled. Type should be `FLOAT`.
        - `target_max` (Required): The maximum value of the target range. This defines the upper limit to which the input value is adjusted. Type should be `FLOAT`.
        - `easing` (Required): A string representing the easing function applied to the distribution of the transformed value, affecting how it is scaled between the source and target ranges. Type should be `COMBO[STRING]`.
    - Outputs:
        - `float`: The input value transformed to fit within the specified target range, potentially altered in distribution by the easing function. Type should be `FLOAT`.
