- `ImpactSEGSOrderedFilter`: The ImpactSEGSOrderedFilter node is designed to filter and order segmentation elements (SEGS) based on specified criteria such as area, width, height, or position. It allows for the selection of a subset of SEGS by ordering them according to the specified criterion and then taking a specified range from the ordered list. This functionality is crucial for scenarios where prioritization or specific ordering of segmentation elements is needed based on their geometric properties or confidence levels.
    - Inputs:
        - `segs` (Required): The segmentation elements (SEGS) to be filtered and ordered. This is the primary input on which the ordering and filtering operations are performed. Type should be `SEGS`.
        - `target` (Required): Specifies the criterion used for ordering the SEGS, such as area, width, height, or specific coordinates. This criterion determines how the SEGS will be sorted before selecting a subset. Type should be `COMBO[STRING]`.
        - `order` (Required): Determines the order in which SEGS are sorted based on the target criterion. A boolean value where True indicates descending order and False indicates ascending order. Type should be `BOOLEAN`.
        - `take_start` (Required): Specifies the starting index from which to begin selecting SEGS after they have been ordered. This allows for skipping a certain number of top elements. Type should be `INT`.
        - `take_count` (Required): Defines the number of SEGS to select starting from the take_start position. This determines the size of the subset of ordered SEGS to be returned. Type should be `INT`.
    - Outputs:
        - `filtered_SEGS`: The subset of SEGS that have been filtered and ordered according to the specified criteria. Type should be `SEGS`.
        - `remained_SEGS`: The SEGS that were not included in the filtered subset, remaining after the ordering and selection process. Type should be `SEGS`.
