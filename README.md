# Image-Compression-Analysis
# Image Compression Analysis: JPEG vs. JPEG2000

A comparative research project implementing and evaluating standard lossy compression techniques using Digital Signal Processing (DSP) principles.

##  Overview
This project explores the mathematical foundations and practical performance of two dominant image compression standards: **JPEG** (Discrete Cosine Transform) and **JPEG2000** (Discrete Wavelet Transform). By manipulating compression parameters, the study analyzes how different algorithms handle information loss at varying scales.



##  Key Features
* **Dual-Algorithm Implementation:** Functional pipelines for both standard JPEG and Wavelet-based (JPEG2000) compression.
* **Variable Quality Testing:** Supports testing across multiple quality levels (10, 50, 90 for JPEG) and compression ratios (5, 10, 20 for JPEG2000).
* **Quantitative Metrics:** Automated calculation of:
    * **PSNR (Peak Signal-to-Noise Ratio):** Measures the ratio between the maximum possible power of a signal and the power of corrupting noise.
    * **SSIM (Structural Similarity Index):** Predicts the perceived quality of digital television and cinematic pictures.
    * **Compression Ratio (CR):** Calculates the percentage of data reduced.
* **Visualization Suite:** Generates side-by-side comparisons, difference images (Original - Compressed), and bar plots for size/quality metrics.



##  Technical Stack
* **Language:** Python 3.x
* **Core Libraries:**
    * `OpenCV`: For JPEG processing and image manipulation.
    * `PyWavelets`: For implementing Wavelet transformations.
    * `NumPy`: For matrix operations and metric calculations.
    * `Matplotlib`: For generating analytical plots.

##  Evaluation Results
Based on the implementation, the results highlight:
1. **Efficiency:** JPEG2000 consistently achieves higher compression ratios but introduces different types of visual artifacts compared to JPEG's blocking effects.
2. **Fidelity:** JPEG maintains superior visual quality at lower compression ratios, while JPEG2000 excels in extreme compression scenarios.

##  How to Run
1. Install dependencies: `pip install opencv-python PyWavelets matplotlib numpy`
2. Run the analysis script: `python compression_analysis.py`
3. View the generated `comparison_results.png` and console output for PSNR/SSIM values.

---
**Developed by:** Habeeban Memon
**Guided by:** Dr. Junaid Ahmed (Sukkur IBA University)
