# 2D-DCT Based Image Compression

##  Overview
This project implements image compression using the **2D Discrete Cosine Transform (DCT)** technique. The approach is based on block-wise processing (8×8) similar to JPEG compression.

The method exploits the energy compaction property of DCT, where most image information is concentrated in low-frequency components.

---

##  Methodology

1. Convert image to grayscale
2. Divide image into 8×8 blocks
3. Apply 2D-DCT to each block
4. Remove small (high-frequency) coefficients
5. Apply inverse DCT (IDCT)
6. Reconstruct compressed image

---

##  Performance Metrics

- **MSE (Mean Square Error)**
- **PSNR (Peak Signal-to-Noise Ratio)**

PSNR is calculated as:

PSNR = 10 * log10(255² / MSE)

---

##  Expected Results

- High PSNR (~40 dB) → good quality
- Lower PSNR (~30 dB) → visible degradation

---

## 🖼️ Output

- Original image
- Compressed image
- MSE and PSNR values

---

##  How to Run

1. Upload an image (`input_image.png`)
2. Run the Python script 
3. View output and saved compressed image

---

##  Key Concept

DCT transforms spatial image data into frequency components:
- Low frequency → important information
- High frequency → less important (can be removed)

---

##  Reference

Y. Sampath Kumar, Rahul Kumar, and Somesh Kumar,  
"2D-Discrete Cosine Transform based Dynamically Controllable Image Compression Technique,"  
IEEE EPTC, 2020.

---

##  Author
Malepati Yashaswi
Prajna H R
