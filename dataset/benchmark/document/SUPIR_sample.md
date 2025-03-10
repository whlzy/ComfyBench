- `SUPIR_sample`: The SUPIR_sample node is designed for sampling in the SUPIR model, utilizing various parameters to control the sampling process. It integrates model loading, latent manipulation, and conditional generation to produce samples based on the provided inputs.
    - Inputs:
        - `SUPIR_model` (Required): The SUPIR model to be used for sampling. It is crucial for defining the generative process. Type should be `SUPIRMODEL`.
        - `latents` (Required): Latent representations to be used as the basis for sampling. These play a key role in the generation process. Type should be `LATENT`.
        - `positive` (Required): Positive conditioning information, guiding the generation towards desired attributes. Type should be `SUPIR_cond_pos`.
        - `negative` (Required): Negative conditioning information, used to steer the generation away from certain attributes. Type should be `SUPIR_cond_neg`.
        - `seed` (Required): A seed for random number generation, ensuring reproducibility of the samples. Type should be `INT`.
        - `steps` (Required): The number of steps to perform in the sampling process. This parameter influences the quality and diversity of the generated samples. Type should be `INT`.
        - `cfg_scale_start` (Required): The initial scaling factor for CFG, affecting the conditioning strength at the beginning of the sampling process. Type should be `FLOAT`.
        - `cfg_scale_end` (Required): The final scaling factor for CFG (Classifier Free Guidance), affecting the conditioning strength at the end of the sampling process. Type should be `FLOAT`.
        - `EDM_s_churn` (Required): A parameter influencing the EDM sampling process, specifically related to churn. Type should be `INT`.
        - `s_noise` (Required): Noise level for the sampling process, affecting the randomness and variability of the generated samples. Type should be `FLOAT`.
        - `DPMPP_eta` (Required): A parameter related to the DPM++ sampling method, influencing its behavior. Type should be `FLOAT`.
        - `control_scale_start` (Required): The initial control scale, influencing the degree of control at the start of the sampling process. Type should be `FLOAT`.
        - `control_scale_end` (Required): The final control scale, determining the degree of control at the end of the sampling process. Type should be `FLOAT`.
        - `restore_cfg` (Required): A flag indicating whether to restore the CFG scale to its original value after sampling. Type should be `FLOAT`.
        - `keep_model_loaded` (Required): A flag indicating whether to keep the model loaded in memory after sampling, which can improve performance for subsequent samples. Type should be `BOOLEAN`.
        - `sampler` (Required): The specific sampler to be used for generating samples, which can vary based on the desired sampling technique. Type should be `COMBO[STRING]`.
        - `sampler_tile_size` (Optional): The size of tiles for the sampler, relevant when sampling is performed in a tiled manner. Type should be `INT`.
        - `sampler_tile_stride` (Optional): The stride of tiles for the sampler, affecting how tiles are overlapped during the sampling process. Type should be `INT`.
    - Outputs:
        - `latent`: The latent representations generated as a result of the sampling process, which may include modifications from the original input latents. Type should be `LATENT`.
