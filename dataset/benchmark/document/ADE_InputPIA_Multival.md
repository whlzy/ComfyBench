- `ADE_InputPIA_Multival`: The node is designed to handle multiple values for PIA (Perceptual Image Annotation) inputs, allowing for the customization and fine-tuning of animation effects in the AnimateDiff framework. It facilitates the integration of varied intensity levels or parameters to influence the animation outcome.
    - Inputs:
        - `multival` (Required): Specifies the intensity level or parameter value for the PIA input, affecting the animation's visual effects. Type should be `MULTIVAL`.
    - Outputs:
        - `pia_input`: Produces a PIA input object configured with the specified multival parameter, ready for use in animation processing. Type should be `PIA_INPUT`.
