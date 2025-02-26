# project-1
# Secret Message Encryption in Images

This project demonstrates how to hide a secret message inside an image using pixel manipulation and later retrieve it using a password-protected decryption process.

## Features
- Encrypts a secret message into an image by modifying pixel values.
- Decrypts the hidden message with the correct password.
- Uses OpenCV for image processing.
- Works in Google Colab for easy execution.

## Requirements
Ensure you have the following dependencies installed:

```bash
pip install opencv-python numpy
```

Or, if using Google Colab, the required libraries are pre-installed.

## How to Use

### 1. Upload an Image
Manually upload an image when prompted in Google Colab.

### 2. Encryption
- Run the script.
- Enter your secret message when prompted.
- Enter a password for decryption security.
- The script embeds the message into the image pixels.
- The encrypted image is saved as `Encryptedmsg.jpg`.

### 3. Decryption
- Enter the correct password.
- If the password is correct, the hidden message is retrieved and displayed.
- If incorrect, access is denied.

## Code Overview

- `cv2.imread()`: Reads the uploaded image.
- `cv2.resize()`: Resizes the image to ensure enough space for the message.
- `for` loop: Iterates through the message and modifies pixel values.
- `cv2.imwrite()`: Saves the modified image.
- `cv2_imshow()`: Displays the encrypted image in Colab.
- Decryption logic verifies the password before extracting the hidden message.

## Limitations
- The message length is restricted by the image size.
- The method does not use cryptographic encryption, making it susceptible to pixel analysis.

## Future Improvements
- Implement stronger encryption techniques (e.g., AES or XOR encoding).
- Support for multiple image formats.
- Improve security to prevent brute-force attacks.

## License
This project is open-source and free to use under the MIT License.

## Author
[Yash Bhavsar

