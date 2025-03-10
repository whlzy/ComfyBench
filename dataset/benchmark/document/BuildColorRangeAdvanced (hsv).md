- `BuildColorRangeAdvanced (hsv)`: The `BuildColorRangeAdvanced (hsv)` node is designed to create a sophisticated range of colors in the HSV color space. It leverages advanced techniques to adjust and fix the bounds of hue, saturation, and value based on given parameters, enabling precise color selection and manipulation for various computer vision tasks.
    - Inputs:
        - `samples` (Required): Specifies the HSV color samples from which to derive the color range. It is essential for determining the base colors for range calculation. Type should be `HSV_SAMPLES`.
        - `hue_exp` (Required): Defines the expression or method to adjust the hue component of the color range. It allows for dynamic hue range adjustments based on specific criteria or algorithms. Type should be `STRING`.
        - `sat_exp` (Required): Specifies the expression or method to adjust the saturation component of the color range. It enables fine-tuning of the saturation levels within the generated color range. Type should be `STRING`.
        - `val_exp` (Required): Indicates the expression or method to adjust the value (brightness) component of the color range. It facilitates the manipulation of brightness levels to achieve the desired color range. Type should be `STRING`.
    - Outputs:
        - `hsv_color`: Returns the calculated HSV color range based on the provided expressions and samples. It represents the final color range after all adjustments have been applied. Type should be `HSV_COLOR`.
        - `combo[string]`: Provides additional information or results related to the color range calculation, potentially including details about the applied adjustments or methods. Type should be `COMBO[STRING]`.
