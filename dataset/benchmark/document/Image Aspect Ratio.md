- `Image Aspect Ratio`: This node calculates the aspect ratio of an image, determining whether it is landscape, portrait, or square based on its width and height. It provides both numerical and common aspect ratio formats, and identifies the image orientation.
    - Inputs:
        - `image` (Optional): The image tensor for which the aspect ratio is to be calculated. If not provided, width and height must be specified. Type should be `IMAGE`.
        - `width` (Optional): The width of the image. Required if the image tensor is not provided. Type should be `NUMBER`.
        - `height` (Optional): The height of the image. Required if the image tensor is not provided. Type should be `NUMBER`.
    - Outputs:
        - `aspect_number`: The numerical aspect ratio of the image. Type should be `NUMBER`.
        - `aspect_float`: The floating-point representation of the image's aspect ratio. Type should be `FLOAT`.
        - `is_landscape_bool`: A boolean indicating if the image is in landscape orientation. Type should be `NUMBER`.
        - `aspect_ratio_common`: The aspect ratio in common format (e.g., '16:9'). Type should be `STRING`.
        - `aspect_type`: A string indicating the type of aspect ratio ('landscape', 'portrait', 'square'). Type should be `STRING`.
