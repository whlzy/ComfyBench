- `CM_IntBinaryCondition`: This node performs binary conditional operations on integer inputs, evaluating the relationship between two integers based on a specified operation (e.g., equality, inequality, greater than, less than). It abstracts the complexity of conditional checks into a simple interface, allowing for easy integration into mathematical and logical workflows.
    - Inputs:
        - `op` (Required): Specifies the binary conditional operation to perform on the integers, such as equality or greater than, and directly influences the outcome of the node's evaluation. Type should be `COMBO[STRING]`.
        - `a` (Required): The first integer operand in the binary conditional operation, serving as one of the two values to be compared. Type should be `INT`.
        - `b` (Required): The second integer operand in the binary conditional operation, serving as the other value to be compared with the first operand. Type should be `INT`.
    - Outputs:
        - `bool`: The result of the binary conditional operation, indicating whether the specified condition holds true between the two integer operands. Type should be `BOOL`.
