- `Repeat Into Grid (image)`: This node tiles input image samples into a grid of configurable dimensions, effectively repeating the input image across a specified number of rows and columns to create a larger, grid-like composite image.
    - Inputs:
        - `image` (Required): The input image to be tiled across the grid. It determines the visual content that will be repeated in each cell of the grid. Type should be `IMAGE`.
        - `columns` (Required): Specifies the number of columns in the grid. This determines how many times the input image is repeated horizontally. Type should be `INT`.
        - `rows` (Required): Specifies the number of rows in the grid. This determines how many times the input image is repeated vertically. Type should be `INT`.
    - Outputs:
        - `image`: The output composite image, consisting of the input image tiled according to the specified rows and columns. Type should be `IMAGE`.
