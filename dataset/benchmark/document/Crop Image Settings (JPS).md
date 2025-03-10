- `Crop Image Settings (JPS)`: The Crop Image Settings node is designed to configure the parameters for cropping images, including the position, offset, and interpolation method. It abstracts the complexity of image cropping settings, allowing for flexible and precise control over how images are cropped and prepared for further processing.
    - Inputs:
        - `source_crop_pos` (Required): Specifies the initial position for cropping the source image. This affects the starting point of the crop and influences the final composition of the cropped image. Type should be `COMBO[STRING]`.
        - `source_crop_offset` (Required): Determines the offset from the specified position for the source image crop, providing fine-tuned control over the crop's placement. Type should be `INT`.
        - `support_crop_pos` (Required): Specifies the initial position for cropping the support image, similar to 'source_crop_pos' but for an additional image or context. Type should be `COMBO[STRING]`.
        - `support_crop_offset` (Required): Determines the offset from the specified position for the support image crop, allowing for precise alignment with the source image. Type should be `INT`.
        - `crop_intpol` (Required): Defines the interpolation method to be used for cropping, affecting the quality and appearance of the cropped image. Type should be `COMBO[STRING]`.
    - Outputs:
        - `cropimage_settings`: The configuration settings for cropping an image, encapsulating position, offset, and interpolation method details. Type should be `BASIC_PIPE`.
