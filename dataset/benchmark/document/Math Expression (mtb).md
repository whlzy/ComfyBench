- `Math Expression (mtb)`: This node is designed to evaluate simple math expressions provided as strings, incorporating the ability to replace placeholders within the expression with specified values. It aims to offer a straightforward method for dynamically calculating numerical results based on input expressions.
    - Inputs:
        - `expression` (Required): The math expression string to be evaluated. This string can include placeholders for dynamic substitution and supports basic math operations. Type should be `STRING`.
    - Outputs:
        - `result (float)`: The evaluated result of the math expression as a floating-point number. Type should be `FLOAT`.
        - `result (int)`: The evaluated result of the math expression, explicitly cast to an integer. Type should be `INT`.
