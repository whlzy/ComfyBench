- `Mask Floor Region`: The Mask Floor Region node is designed to process input masks and apply a specific floor region masking operation. This operation identifies and isolates the floor regions within the given masks, transforming them into a format suitable for further analysis or processing.
    - Inputs:
        - `masks` (Required): The 'masks' parameter represents the input masks on which the floor region detection and isolation will be performed. It is crucial for identifying the specific areas within the images that correspond to floor regions. Type should be `MASK`.
    - Outputs:
        - `MASKS`: The output is a tensor containing the processed masks with the floor regions isolated, ready for further analysis or processing. Type should be `MASK`.
