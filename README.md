# DIP-Project
Image Denoising using Wavelet Transform
# Image Denoising using Wavelet Transform

This project explores image denoising techniques using wavelet transforms, with a focus on **BayesShrink** and **VisuShrink** thresholding methods. The goal is to remove noise while preserving important image details such as edges and textures.

##  Overview

Images captured in real-world environments often contain noise due to lighting, sensor imperfections, or transmission. Denoising is essential before applying further processing tasks like segmentation or classification.

This work demonstrates how **discrete wavelet transform (DWT)** can decompose an image into different frequency sub-bands and how applying adaptive thresholding techniques helps in reducing noise efficiently.

##  Methodology

1. Load and normalize grayscale image.
2. Add Gaussian noise to simulate real-world conditions.
3. Apply 1-level and 2-level wavelet decomposition using the Haar wavelet.
4. Estimate noise using the MAD method from high-frequency subbands.
5. Perform denoising using:
   - BayesShrink (adaptive)
   - VisuShrink (universal threshold)
6. Evaluate performance using **Peak Signal-to-Noise Ratio (PSNR)**.
7. Visualize results and compare denoising efficiency.

##  Folder Structure


All output results, including intermediate denoised images and PSNR comparisons, are stored in the `RESULTS` folder.

##  Sample Results

- BayesShrink PSNR: 27.29 dB
- VisuShrink (σ/4) PSNR: 25.59 dB

BayesShrink provided the best balance between noise suppression and detail retention in our experiments.

##  Libraries Used

- Python 3.x
- OpenCV
- NumPy
- PyWavelets
- Matplotlib
- scikit-image

##  Applications

- Medical Image Enhancement
- Satellite Image Preprocessing
- OCR Systems
- Low-light Photography
- Surveillance Image Enhancement

##  Future Scope

Future improvements may include hybrid methods combining wavelets with CNNs or transformer-based models, testing on real-world noise datasets (like SIDD or DND), and developing real-time denoising pipelines.

##  Authors

- Megha S Lekshmi (M241085EC) – megha_m241085ec@nitc.ac.in  
- Haneena Sajan (M241294EC) – haneena_m241294ec@nitc.ac.in  
M.Tech Signal Processing, NIT Calicut

---

