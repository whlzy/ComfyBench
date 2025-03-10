- `ImageConstantHSV`: The ImageConstantHSV node generates constant color images based on specified HSV (Hue, Saturation, Value) color values. It allows for the creation of uniform color images with adjustable color properties, enabling the generation of images with precise color tones.
    - Inputs:
        - `width` (Required): Specifies the width of the generated image. It determines the horizontal dimension of the output image. Type should be `INT`.
        - `height` (Required): Specifies the height of the generated image. It determines the vertical dimension of the output image. Type should be `INT`.
        - `batch_size` (Required): Determines the number of images to generate in a single batch. This allows for the generation of multiple images with the same color properties simultaneously. Type should be `INT`.
        - `hue` (Required): Sets the hue component of the HSV color model for the image, defining the color tone. Type should be `FLOAT`.
        - `saturation` (Required): Sets the saturation component of the HSV color model, controlling the intensity of the color. Type should be `FLOAT`.
        - `value` (Required): Sets the value component of the HSV color model, determining the brightness of the color. Type should be `FLOAT`.
    - Outputs:
        - `image`: The generated image(s) with constant color based on the specified HSV values. Type should be `IMAGE`.
