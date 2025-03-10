- `LayerColor_ AutoBrightness`: The AutoBrightness node automatically adjusts the brightness of an image based on specified strength and saturation levels, optionally considering a mask to apply the adjustment selectively.
    - Inputs:
        - `image` (Required): The image to be processed for auto brightness adjustment. It serves as the primary input for the node's operation. Type should be `IMAGE`.
        - `strength` (Required): Determines the intensity of the brightness adjustment. A higher value results in a more pronounced change. Type should be `INT`.
        - `saturation` (Required): Adjusts the saturation level of the image alongside brightness, allowing for a balanced color correction. Type should be `INT`.
        - `mask` (Optional): An optional mask that can be applied to restrict the brightness adjustment to specific areas of the image. Type should be `MASK`.
    - Outputs:
        - `image`: The output image after auto brightness adjustment, reflecting changes in brightness and saturation. Type should be `IMAGE`.
