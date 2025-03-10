- `RemapToOuterCylinder`: The RemapToOuterCylinder node is designed to transform an image by mapping it onto the surface of an imaginary outer cylinder. This transformation is based on the field of view and an optional swap of the x and y axes, aiming to simulate a perspective where the image wraps around the viewer in a cylindrical manner.
    - Inputs:
        - `fov` (Required): The field of view in degrees, determining the extent of the cylindrical projection. It influences the curvature and the scale of the remapped image. Type should be `INT`.
        - `swap_xy` (Required): A boolean flag that, when true, swaps the x and y axes in the output mapping. This can be used to adjust the orientation of the remapped image based on specific requirements. Type should be `BOOLEAN`.
    - Outputs:
        - `remap`: The output of the RemapToOuterCylinder node is a transformed image that has been remapped to simulate being wrapped around an outer cylinder. This output is crucial for applications requiring cylindrical perspective transformations. Type should be `REMAP`.
