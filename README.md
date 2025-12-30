<div align="center">

# 🌌 Astronomical Image Denoising and Enhancement

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Astropy](https://img.shields.io/badge/Powered%20by-Astropy-orange.svg)](https://www.astropy.org/)
[![Colab](https://img.shields.io/badge/Open%20in-Colab-yellow.svg)](https://colab.research.google.com/)

**Advanced image processing pipeline for denoising and enhancing astronomical images from the Hubble Space Telescope**

</div>

---

## 📖 Overview

This project implements a comprehensive image processing pipeline designed to denoise and enhance astronomical images captured by the Hubble Space Telescope. By combining classical signal processing techniques with modern deep learning approaches, we aim to recover faint celestial structures (stars, galaxies, dust lanes) that are often obscured by instrumental and observational noise.

## ✨ Key Features

- 🔭 **FITS Image Processing** - Native support for astronomical FITS format
- 🧹 **Advanced Denoising** - Multiple filtering techniques for noise reduction
- 🤖 **Deep Learning Models** - U-Net and autoencoder architectures
- 📊 **Comparative Analysis** - Benchmark classical vs. ML methods
- 🎯 **Structure Preservation** - Maintain astronomical features while reducing noise
- 📈 **Quantitative Metrics** - SNR, PSNR, and SSIM evaluation

## 🎯 Objectives

- Remove additive noise from FITS images of galaxies (e.g., M51 - Whirlpool Galaxy)
- Enhance faint astronomical signals while preserving structural integrity
- Compare performance of classical filters vs. deep learning methods
- Develop a robust pipeline for automated astronomical image enhancement

## 🔬 Data Source

Images are obtained from the [Hubble Legacy Archive](https://hla.stsci.edu/), with primary focus on:
- **Filter**: F555W (green light / V-band)
- **Targets**: Nearby galaxies, nebulae, and star clusters
- **Format**: FITS (Flexible Image Transport System)

## 🛠️ Technology Stack

### Core Libraries
- **Python 3.8+** - Primary programming language
- **Astropy** - FITS file handling and astronomical utilities
- **NumPy** - Numerical computations
- **Matplotlib** - Data visualization

### Deep Learning (Planned)
- **TensorFlow / Keras** - U-Net implementation
- **PyTorch** - Autoencoder models
- **scikit-image** - Classical image processing

### Development Environment
- **Google Colab** - Cloud-based development and training
- **Jupyter Notebooks** - Interactive experimentation

## 📁 Project Structure

```
Astronomical-Image-Denoising-and-Enhancement/
├── notebooks/          # Jupyter/Colab notebooks
│   ├── preprocessing.ipynb
│   ├── classical_methods.ipynb
│   └── deep_learning.ipynb
├── data/              # Sample FITS images
│   ├── raw/
│   └── processed/
├── models/            # Trained model weights
├── src/               # Source code modules
├── results/           # Output images and metrics
└── README.md
```

## 🚀 Getting Started

### Prerequisites

```bash
Python 3.8 or higher
pip or conda package manager
```

### Installation

```bash
# Clone the repository
git clone https://github.com/Polisetty-Cyril/Astronomical-Image-Denoising-and-Enhancement.git
cd Astronomical-Image-Denoising-and-Enhancement

# Install required packages
pip install astropy matplotlib numpy scipy scikit-image

# For deep learning (optional)
pip install tensorflow torch torchvision
```

### Quick Start

```python
# Load and process a FITS image
from astropy.io import fits
import matplotlib.pyplot as plt

# Load image
hdu = fits.open('data/galaxy_m51.fits')
image_data = hdu[0].data

# Display
plt.imshow(image_data, cmap='gray')
plt.title('M51 Galaxy - Raw Image')
plt.show()
```

## 📊 Methodology

### Classical Approaches
- Gaussian filtering
- Median filtering
- Wiener filtering
- Wavelet denoising

### Deep Learning Approaches
- **U-Net Architecture** - Encoder-decoder with skip connections
- **Convolutional Autoencoders** - Learned feature extraction
- **Residual Learning** - Direct noise prediction

## 📈 Results

*Results and performance metrics will be updated as the project progresses.*

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Polisetty Cyril**
- Undergraduate researcher specializing in astronomical image processing and data science
- Interested in computer vision, deep learning, and astrophysics

## 🙏 Acknowledgments

- [Hubble Space Telescope](https://hubblesite.org/) for the amazing imagery
- [STScI](https://www.stsci.edu/) for maintaining the Hubble Legacy Archive
- The Astropy community for excellent tools and documentation

## 📧 Contact

For questions or collaboration opportunities, please open an issue or reach out via GitHub.

---

<div align="center">
Made with ❤️ and ☕ for the astronomical community
</div>
