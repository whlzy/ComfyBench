- `BboxDetectorCombined_v2`: This node combines bounding box detection with segmentation mask creation and optional dilation, providing a comprehensive solution for object detection and segmentation in images. It leverages a bounding box model to detect objects and generate segmentation masks, which can then be optionally dilated for improved coverage or specificity.
    - Inputs:
        - `bbox_detector` (Required): Specifies the bounding box model to be used for object detection. It plays a crucial role in identifying objects within the image and generating initial bounding boxes. Type should be `BBOX_DETECTOR`.
        - `image` (Required): The input image on which object detection and segmentation are to be performed. It serves as the primary data source for the detection process. Type should be `IMAGE`.
        - `threshold` (Required): A threshold value to filter detected objects based on confidence scores. It helps in eliminating detections with low confidence. Type should be `FLOAT`.
        - `dilation` (Required): Determines the extent to which the segmentation masks are dilated. This can enhance the mask's coverage over the detected objects. Type should be `INT`.
    - Outputs:
        - `mask`: The output segmentation mask representing detected objects. It combines all individual object masks into a single mask layer. Type should be `MASK`.
