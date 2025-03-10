- `INPAINT_ApplyFooocusInpaint`: This node applies a specialized inpainting technique using the Fooocus method to enhance or modify images based on provided patches and latent information. It integrates seamlessly with the inpainting process, leveraging learned features and adjustments to achieve high-quality inpainting results.
    - Inputs:
        - `model` (Required): The model parameter represents the base model to which the inpainting patches and adjustments will be applied. It is crucial for defining the starting point of the inpainting process. Type should be `MODEL`.
        - `patch` (Required): This parameter consists of the inpainting head model and the LoRA patch information, which are essential for applying the specific inpainting adjustments to the base model. Type should be `INPAINT_PATCH`.
        - `latent` (Required): The latent parameter contains the latent representation and noise mask of the image to be inpainted, providing the necessary context for the inpainting operation. Type should be `LATENT`.
    - Outputs:
        - `model`: Returns a modified version of the base model with inpainting patches applied, ready for further inpainting tasks. Type should be `MODEL`.
