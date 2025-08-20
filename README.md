Project Overview: 
This project focuses on converting hand-drawn or edge-based sketches into high-resolution, photorealistic human faces using a Conditional Generative Adversarial Network (cGAN). Unlike standard sketch-to-image translation, our approach incorporates facial attributes (e.g., gender, smile, glasses, hair color) as conditional vectors, ensuring that the generated face aligns with both the sketch structure and the desired attributes.

Key Features

1) Dual-Branch Generator:
   Branch 1: Encodes the input sketch.
   Branch 2: Encodes attribute vectors (40 attributes from CelebA).
   The branches are fused to generate realistic face images.

2) Conditional Discriminator: Distinguishes between real and generated images while ensuring attribute alignment.

3) High-Resolution Outputs: Generates photorealistic faces conditioned on sketches + attributes.

4) Trained on CelebA Dataset: Utilized 200K+ celebrity images with annotated attributes.

5) Optimized Training:
   Optimizer: Adam (lr = 0.0002, β1 = 0.5)
   Batch Size: 64
   Epochs: 200
   Hardware: NVIDIA Tesla P100 GPU
