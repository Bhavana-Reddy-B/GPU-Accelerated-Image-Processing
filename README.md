# ⚡ GPU-Accelerated Image Processing Pipeline

[![Python Version](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://www.python.org/downloads/)

## 🧠 Overview

**GPU-Accelerated Image Processing Pipeline** is a high-performance image transformation and filtering project built using **OpenCV** with **CUDA** acceleration.  
It demonstrates how GPU computing can significantly speed up image operations like blurring, edge detection, color conversion, and resizing — especially for large batches of high-resolution images.

Originally developed for experimentation on Google Colab, this version refactors and extends the pipeline to benchmark **GPU vs CPU performance** for real-time image processing tasks.

---

## 🚀 Features

- ⚙️ **GPU-Accelerated Processing:** Uses CUDA-enabled OpenCV functions for high-speed filtering and transformations.  
- 🧩 **Real-Time Comparison:** Benchmarks GPU vs CPU execution times for common image processing operations.  
- 🖼️ **Multi-Filter Support:** Includes operations such as Gaussian blur, edge detection, color space conversion, and thresholding.  
- 📊 **Performance Visualization:** Displays performance metrics and speedup ratios for each operation.  
- ☁️ **Colab Compatible:** Fully runnable in Google Colab with CUDA-enabled runtimes.

---

## 📦 Tech Stack

- **Python 3.8+**  
- **OpenCV (CUDA-enabled build)**  
- **NumPy**  
- **Matplotlib** (for performance plots)  
- **Google Colab / Jupyter**  

---

## 🧩 Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Bhavana-Reddy-B/GPU-Accelerated-Image-Processing.git
cd GPU-Accelerated-Image-Processing
```

### 2️⃣ Set up environment
```bash
pip install -r requirements.txt
```

### 3️⃣ Verify CUDA and OpenCV GPU support
```python
import cv2
print(cv2.getBuildInformation())
```
You should see `CUDA: YES` in the build info.

---

## ⚡ Usage

### Run on Google Colab
1. Upload the notebook to Google Colab.  
2. Set the runtime to **GPU** (Runtime → Change runtime type → GPU).  
3. Execute all cells to compare CPU vs GPU processing speeds.

### Run locally
1. Ensure your system has an NVIDIA GPU with CUDA drivers installed.  
2. Run the Python script:
```bash
python gpu_image_processing.py
```
3. View generated output images and performance logs.

---

## 📁 Project Structure

| File | Description |
|------|--------------|
| `gpu_image_processing.py` | Main script for image processing and benchmarking. |
| `requirements.txt` | List of Python dependencies. |
| `images/` | Folder to store sample images. |
| `results/` | Contains output images and performance graphs. |

---

## 📊 Example Output

| Operation | CPU Time (ms) | GPU Time (ms) | Speedup |
|------------|---------------|---------------|----------|
| Gaussian Blur | 120 | 15 | 8× |
| Edge Detection | 95 | 10 | 9.5× |
| Color Conversion | 60 | 8 | 7.5× |

*Performance will vary depending on GPU hardware and image resolution.*

---

## 👨‍💻 Author

Developed by [Bhavana Reddy](https://github.com/Bhavana-Reddy-B)  
