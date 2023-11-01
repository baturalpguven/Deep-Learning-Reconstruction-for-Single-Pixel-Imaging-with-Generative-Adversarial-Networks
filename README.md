# Deep-Learning-Reconstruction-for-Single-Pixel-Imaging-with-Generative-Adversarial-Networks
Single pixel imaging (SPI) enables high-resolution imaging through multiple coded measurements based on low-resolution snapshots. An inverse problem can then be solved to reconstruct a high-resolution image given the coded measurements. There has been recent interest in adoption of deep neural networks in SPI reconstruction. However, existing methods are commonly trained with pixel-wise loss terms such as the ℓ 1 -norm loss, which can result in spatial blurring and poor sensitivity to structural details. In this study, we propose a novel approach for deep SPI reconstruction based on an unrolled conditional generative adversarial network (cGAN) model. The generator estimates the high-resolution image using coded low-resolution measurements by iterating across a cascade of denoising and data-consistency modules. Meanwhile, the discriminator distinguishes real versus synthesized high-resolution images. The architecture is trained end-to-end via a combined pixel-wise and adversarial loss to enhance sensitivity to structural details. The proposed method is demonstrated against existing SPI reconstruction methods, and ablation studies are performed to demonstrate the individual model components. The proposed method outperforms competing methods in terms of both quantitative metrics and visual quality.


## Proposed Architecture

<div align="center">
  <img src="https://github.com/baturalpguven/Deep-Learning-Reconstruction-for-Single-Pixel-Imaging-with-Generative-Adversarial-Networks/assets/77858949/a08fe7f5-0563-418a-917f-d98dd2e20f5d" alt="Figure 1: Proposed Architecture">
  <p><em>Figure 1: Schematic of the proposed model. First, a least-squared estimate of the scene from the measured data is computed. The estimate
 is then iteratively regularized using a deep denoiser followed by a least-squares-based data consistency (DC) projection. The reconstructed
 scenes are processed via a discriminator to compute adversarial loss. The entire model is trained end-to-end via a linear combination of
 adversarial and pixel-wise ℓ1-norm losses.</em></p>
</div>

## Results

<div align="center">
  <img src="https://github.com/baturalpguven/A-Diffusion-Based-Reconstruction-Technique-for-Single-Pixel-Camera/assets/77858949/accfc9bf-3972-462c-82c5-4a2ef82619df.png](https://github.com/baturalpguven/Deep-Learning-Reconstruction-for-Single-Pixel-Imaging-with-Generative-Adversarial-Networks/assets/77858949/bd8dd0f0-67c3-40b6-a7ad-0b37af835b4a" alt="Figure 2: Reconstruction Results">
  <p><em>Figure 2: (a) Ground truth image. Reconstructed images using (b) TV, (c) a TVFL1, (d) PnP, (e) Only ℓ1-loss (ablated variant of the proposed method), and (f) the proposed method.</em></p>
</div>



<div align="center">
  <img src="https://github.com/baturalpguven/Deep-Learning-Reconstruction-for-Single-Pixel-Imaging-with-Generative-Adversarial-Networks/assets/77858949/2b58b6db-b1c4-4f20-b4d2-ffb52d64e6e4" alt="Figure 2: Reconstruction Results">
  <p><em>Figure 3: Performance of ablated variants of the proposed method. ( We examined
 the value of adversarial loss by constructing a variant that
 used an ℓ1-loss term (Only ℓ1-loss). We examined the value
 of Wasserstein GAN (WGAN) training by constructing a
 variant that used regular GAN training (GAN-based). We
 examined the value of the data consistency (DC) module
 by constructing a variant that omitted the DC projections
 (DC-ablated). Finally, we examined the value of iteratively
 ϵi by constructing a variant that used fixed ϵi (Fixed
 DC).</em></p>
</div>

![image](https://github.com/baturalpguven/Deep-Learning-Reconstruction-for-Single-Pixel-Imaging-with-Generative-Adversarial-Networks/assets/77858949/f58e0aa6-da5e-48f8-adfd-b155f7022aeb)



<div align="center">
  <img src="https://github.com/baturalpguven/Deep-Learning-Reconstruction-for-Single-Pixel-Imaging-with-Generative-Adversarial-Networks/assets/77858949/f58e0aa6-da5e-48f8-adfd-b155f7022aeb" alt="Figure 2: Reconstruction Results">
  <p><em>Figure 4: Performance of competing methods </em></p>
</div>

## Link

For more details, please refer to the [IEEE Xplore document](https://ieeexplore.ieee.org/document/10223149) on the Deep Learning Reconstruction for Single Pixel Imaging with Generative Adversarial Networks.

