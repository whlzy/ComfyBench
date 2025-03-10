- `LayerColor_ RGB`: This node is designed for color correction in RGB color space, allowing adjustments to the red, green, and blue channels of an image. It enables fine-tuning of the image's color balance by applying specific offsets to each color channel, enhancing or modifying the image's overall coloration.
    - Inputs:
        - `image` (Required): The input image to be color corrected. It serves as the base for applying RGB adjustments, impacting the visual outcome of the color correction process. Type should be `IMAGE`.
        - `R` (Required): The offset value for the red channel, which adjusts the intensity of red colors in the image. This parameter directly influences the image's red hues, allowing for nuanced color correction. Type should be `INT`.
        - `G` (Required): The offset value for the green channel, which adjusts the intensity of green colors in the image. This parameter is crucial for modifying the image's green hues, enabling detailed color adjustments. Type should be `INT`.
        - `B` (Required): The offset value for the blue channel, which adjusts the intensity of blue colors in the image. By altering this parameter, users can fine-tune the blue hues within the image, achieving desired color effects. Type should be `INT`.
    - Outputs:
        - `image`: The color-corrected image, with adjustments applied to the red, green, and blue channels. This output reflects the cumulative effect of the RGB offsets on the original image, showcasing the enhanced or altered coloration. Type should be `IMAGE`.
