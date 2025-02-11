# QR Code Generator

This Python script generates a QR code from a given data input and saves it as an image file (default is qrcode.png). The script uses the qrcode library to create the QR code and save it as a PNG file.

## Prerequisites
Make sure you have the following installed:
  Python 3.x
  qrcode library (can be installed via pip)
  
To install the required dependencies, run:
```sh
   pip install qrcode
   ```

## Features
- Takes input data from the user.
- Allows specifying the output filename for the QR code image.
- Saves the generated QR code as a .png image.
- Configurable parameters for the QR code generation such as error correction, box size, and border thickness.

## How to Use
Clone or download this repository.

Run the script by executing:

```sh
   python generate_qr_code.py
   ```
You will be prompted to enter:

1. The data to encode in the QR code (e.g., a URL, text, or any other data).
2. The filename to save the QR code (must end with .png).
3. The script will generate and save the QR code as a PNG image in the specified filename.

### Example
1. Enter the data to encode in the QR code: https://www.example.com
2. Enter the filename to save the QR code (with .png extension): example_qr.png
3. QR Code generated and saved as example_qr.png
The generated image file will be saved with the name example_qr.png (or whatever you specify) in the current directory.

## Customization
You can customize the following parameters in the generate_qr_code function:

- version: Controls the size of the QR code (from 1 to 40).
- error_correction: Controls the error correction level. Use constants like:
- ERROR_CORRECT_L: 7% of data can be restored.
- ERROR_CORRECT_M: 15% of data can be restored.
- ERROR_CORRECT_Q: 25% of data can be restored.
- ERROR_CORRECT_H: 30% of data can be restored.
- box_size: Controls how many pixels each box of the QR code is.
- border: Controls the thickness of the border around the QR code.

## License
This project is licensed under the MIT License
