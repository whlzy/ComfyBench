- `ImpactSegsAndMask`: The node applies a bitwise AND operation between segmentation masks and a given mask, modifying the segmentation data based on the overlap with the mask. This operation is useful for refining segmentation results by incorporating additional mask information, enhancing the accuracy and relevance of the segmented output.
    - Inputs:
        - `segs` (Required): The segmentation data to be refined. It plays a crucial role in determining the final output by providing the initial set of segments to be modified. Type should be `SEGS`.
        - `mask` (Required): The mask to apply to the segmentation data. It affects the operation by defining which parts of the segments will be retained or discarded based on the bitwise AND operation. Type should be `MASK`.
    - Outputs:
        - `segs`: The modified segmentation data after applying the bitwise AND operation with the given mask. It represents the refined set of segments that have been altered based on the mask's criteria. Type should be `SEGS`.
