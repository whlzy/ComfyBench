- `CM_BoolUnaryOperation`: This node performs unary boolean operations on a given boolean value. It supports operations like logical NOT, allowing for the manipulation of boolean logic in a mathematical or logical context.
    - Inputs:
        - `op` (Required): Specifies the unary boolean operation to be performed, such as 'Not'. This choice determines how the input boolean value is manipulated. Type should be `COMBO[STRING]`.
        - `a` (Required): The boolean value to be operated on. This is the primary input for the unary operation. Type should be `BOOL`.
    - Outputs:
        - `bool`: The result of the unary boolean operation performed on the input value. Type should be `BOOL`.
