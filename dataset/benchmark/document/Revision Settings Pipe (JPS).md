- `Revision Settings Pipe (JPS)`: The Revision Settings Pipe node is designed to process and adjust image revision settings, facilitating the customization of image processing parameters such as cropping, interpolation, and noise augmentation. It serves as a configurable pipeline component within image processing workflows, enabling precise control over the revision effects applied to images.
    - Inputs:
        - `revision_settings` (Required): Specifies the settings for image revision, including resolution, interpolation method, cropping preferences, offsets, strengths, and noise augmentation levels. This input is crucial for determining how the image will be modified during the revision process. Type should be `BASIC_PIPE`.
    - Outputs:
        - `crop_res`: The resolution to which the image will be cropped. Type should be `INT`.
        - `crop_intpol`: The interpolation method used for cropping the image. Type should be `COMBO[STRING]`.
        - `rev1_crop`: Specifies the first revision cropping preference. Type should be `COMBO[STRING]`.
        - `rev1_offset`: The offset applied during the first revision. Type should be `INT`.
        - `rev2_crop`: Specifies the second revision cropping preference. Type should be `COMBO[STRING]`.
        - `rev2_offset`: The offset applied during the second revision. Type should be `INT`.
        - `rev1_strength`: The strength of the first revision effect. Type should be `FLOAT`.
        - `rev2_strength`: The strength of the second revision effect. Type should be `FLOAT`.
        - `rev1_noiseaug`: The level of noise augmentation applied during the first revision. Type should be `FLOAT`.
        - `rev2_noiseaug`: The level of noise augmentation applied during the second revision. Type should be `FLOAT`.
