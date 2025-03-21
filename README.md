# ✨ Number Plate Detection and OCR ✨

This repository contains a Python script for detecting and extracting text from vehicle number plates using OpenCV and Tesseract OCR. The code preprocesses an image, detects the number plate region, and performs OCR to extract and clean the text.

## 🔧 Features

- ✔️ Image preprocessing: grayscale conversion, Gaussian blur, and adaptive thresholding.
- ✔️ Contour detection for locating number plates.
- ✔️ Optical Character Recognition (OCR) using Tesseract.
- ✔️ Configurable to work with different input images.

## ⚡️ Prerequisites

To use this project, ensure the following dependencies are installed:

- 👤 Python 3.7 or higher
- 🔨 OpenCV (`cv2`)
- 🔨 pytesseract
- 🔨 matplotlib (optional, for additional debugging or visualization)
- 🔨 Tesseract-OCR (external software)

### ⚙️ Installing Dependencies

Install the required Python packages using `pip`:

```bash
pip install opencv-python pytesseract matplotlib
```

### ✔️ Installing Tesseract-OCR

Download and install [Tesseract-OCR](https://github.com/tesseract-ocr/tesseract). Make sure to set the `tesseract_cmd` path in the script to match your installation.

For example:
```python
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
```

## 🔄 Usage

1. 🔧 Clone the repository:

```bash
git clone https://github.com/your-username/number-plate-detection.git
cd number-plate-detection
```

2. 🌐 Add your input images to the project directory or provide a path to the images.

3. 🔍 Modify the `image_path` variable in the `main()` function to point to your test image.

Example:
```python
image_path = r'C:\Users\user\Downloads\np1.jpeg'
```

4. ⚙️ Run the script:

```bash
python number_plate_detection.py
```

5. ✨ The program will process the image, detect the number plate, and display the extracted text.

## 🎨 Example Output

### 🔍 Detected Number Plate
The script will draw a green contour around the detected number plate region and display the processed image.

### 🔒 OCR Result
The extracted text will be printed to the console:

```text
Detected Number Plate: ABC1234
```

## 🗋 File Overview

- **number_plate_detection.py**: The main Python script for detecting and extracting number plate text.

## ⚠️ Troubleshooting

- ⛔️ Ensure Tesseract-OCR is installed and the path is correctly set in the script.
- 🔗 For best results, use high-quality images with clear number plates.
- ⚙️ If detection fails, experiment with preprocessing parameters like Gaussian blur, adaptive thresholding, or contour area filtering.

## ❤️ License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## 📢 Contributing

Feel free to submit issues or pull requests to improve the code or add new features!

---

### 🙏 Acknowledgments

- [OpenCV](https://opencv.org/)
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract)
