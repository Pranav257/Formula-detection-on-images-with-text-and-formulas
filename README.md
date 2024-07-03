 

# Image to LaTeX Conversion Tool

This Python tool extracts both regular text and LaTeX formulas from images. It utilizes the `pytesseract` library for OCR (Optical Character Recognition) to extract text and the `pix2tex` library for specialized LaTeX formula extraction.

## Prerequisites

Before you can run this script, you need to install the necessary Python libraries and system packages. Here's how you can install them:

### Python Libraries

Install `pytesseract` and the PIL (Pillow) library using pip:

```bash
pip install pytesseract pillow
```

### System Packages

The `tesseract-ocr` package is required for `pytesseract` to function. Install it using:

```bash
sudo apt install tesseract-ocr
```

### LaTeX OCR Model

Install `pix2tex` via pip to enable LaTeX formula extraction:

```bash
pip install pix2tex
```

Ensure that you have LaTeX installed in your system for `pix2tex` to work properly. It can be installed with the following command:

```bash
sudo apt install texlive
```

## Usage

To use this script, you will need to have an image file containing text and/or LaTeX formulas. Here's a simple way to run the script:

1. Place your image file in a known directory.
2. Update the `image_path` variable in the script to the location of your image file.
3. Run the script to see the extracted text and formulas.

Example command:

```python
image_path = 'path/to/your/image.png'
latex_content = image_to_latex(image_path)
print(latex_content)
```

## Output

The script outputs the extracted regular text and LaTeX formulas. If any errors occur during extraction, they will be printed to the console.

## Limitations

- The accuracy of text and formula extraction depends heavily on the quality of the input image.
- The script currently assumes that the image contains a single block of text and formulas. Multiple blocks may require additional handling.

## Contributing

Contributions to improve the script are welcome. Please fork the repository and submit a pull request with your enhancements.
 
