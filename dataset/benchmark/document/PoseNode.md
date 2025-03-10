- `PoseNode`: The PoseNode is designed to process images by converting them into a tensor format suitable for pose estimation tasks. It emphasizes the preparation of image data for further analysis or model inference, focusing on the transformation of images from their original format into a normalized tensor representation.
    - Inputs:
        - `image` (Required): The 'image' parameter represents the name of the image file to be processed. It is crucial for locating and loading the image from a temporary directory, where it undergoes conversion and normalization for pose analysis. Type should be `COMBO[STRING]`.
    - Outputs:
        - `image`: The output is a tensor representation of the input image, prepared for pose estimation tasks. This tensor is normalized and ready for further processing or model inference. Type should be `IMAGE`.
