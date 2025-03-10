- `BboxVisualize`: The BboxVisualize node is designed to overlay bounding boxes on images, enhancing visual analysis by clearly delineating detected objects or areas of interest. It operates by drawing colored lines around specified regions, facilitating the evaluation of object detection models or the visualization of spatial data within images.
    - Inputs:
        - `images` (Required): A batch of images on which bounding boxes will be drawn. This input is essential for visualizing how well detected regions align with the objects or areas of interest in the images. Type should be `IMAGE`.
        - `bboxes` (Required): A list of bounding box coordinates specifying the regions to be highlighted on the images. Each bounding box is defined by its top-left corner coordinates, width, and height, which are crucial for accurately drawing the boxes on the corresponding images. Type should be `BBOX`.
        - `line_width` (Required): Specifies the thickness of the lines used to draw the bounding boxes. Adjusting this parameter allows for customization of the visualization's appearance, making the bounding boxes more or less prominent. Type should be `INT`.
    - Outputs:
        - `images`: A batch of images with bounding boxes drawn over them, facilitating visual inspection of detected regions or areas of interest. Type should be `IMAGE`.
