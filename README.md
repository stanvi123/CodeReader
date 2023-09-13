# myrichpanel

# Image Text Extraction using pytesseract

This Python script allows you to extract text from images using the pytesseract library. It is particularly useful for tasks such as reading text from scanned documents, screenshots, or any images containing textual content.

## Prerequisites

Before running the code, ensure you have the following installed:

- Python 3.x
- [Tesseract OCR](https://github.com/tesseract-ocr/tesseract) installed and configured. You may need to set the path to the Tesseract executable in the code.

## Installation

You can install the required Python libraries using pip:

```bash
pip install pytesseract
pip install pillow
```

## Usage

1. Modify the `pytesseract.pytesseract.tesseract_cmd` variable in the code to point to the Tesseract executable on your system.

```python
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
```

2. Specify the directory containing the images you want to process by setting the `image_folder` variable:

```python
image_folder = "path_to_your_task2_folder"
```

3. Run the script. It will process all image files (with extensions .jpg, .png, .jpeg) in the specified folder and extract text from each image.

```bash
python your_script.py
```

4. The extracted text will be displayed in the console, along with the image path.

```plaintext
Image Path: path_to_image/image1.jpg
Extracted Text:
This is the extracted text from image1.

Image Path: path_to_image/image2.png
Extracted Text:
Text from image2 goes here.
```

## Notes

- Ensure that your images are clear and contain legible text for better extraction results.
- You can customize the code further for your specific use case, such as saving the extracted text to a file or integrating it into a larger project.
