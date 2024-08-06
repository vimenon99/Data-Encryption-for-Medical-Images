# Cryptographic and Image Processing Project

This project involves a series of cryptographic and image processing tasks, including RSA key pair generation, DNA encoding/decoding, image steganography, and wavelet compression. The goal is to demonstrate various techniques in data security and image processing.

## Key Components

1. **RSA Key Pair Generation**:
   - Generates RSA private and public keys.
   - Saves keys to PEM files.

2. **DNA Encoding**:
   - Encodes messages into DNA sequences using a predefined mapping.

3. **RSA Signature**:
   - Signs AES-encrypted messages with RSA private keys.

4. **Image Steganography**:
   - Embeds signed AES-encrypted messages into images.
   - Calculates PSNR to evaluate image quality.

5. **Wavelet Compression**:
   - Applies wavelet transform to compress images.
   - Plots compression results.

6. **Image Decoding and Signature Verification**:
   - Decodes embedded messages from images.
   - Verifies signatures using RSA public keys.

7. **AES Decryption**:
   - Decrypts AES-encrypted messages.

8. **Reversing DNA Encoding**:
   - Converts DNA sequences back to original messages.

9. **Tic-Tac-Toe Board Initialization**:
   - Initializes a game board for potential machine learning applications.

## Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/yourrepository.git
    ```

2. **Install dependencies**:
    ```bash
    pip install pycryptodome pandas cryptography pillow stepic opencv-python pywavelets matplotlib tensorflow
    ```

## Usage

1. **Generate RSA Keys**:
    ```python
    from your_script import generate_rsa_key_pair, save_private_key_to_file, save_public_key_to_file
    private_key, public_key = generate_rsa_key_pair()
    save_private_key_to_file(private_key, 'private_key.pem')
    save_public_key_to_file(public_key, 'public_key.pem')
    ```

2. **Encode and Decode Messages**:
    ```python
    from your_script import encode_to_dna, decode_dna, AESCipher
    message = "Your message here"
    encoded_dna = encode_to_dna(message)
    decoded_message = decode_dna(encoded_dna)
    ```

3. **Steganography and Compression**:
    ```python
    from your_script import encode_image, calculate_psnr, compress_image
    encode_image('path/to/image.jpg', 'path/to/output.png')
    psnr = calculate_psnr('path/to/original.jpg', 'path/to/output.png')
    compress_image('path/to/image.jpg', threshold=50)
    ```

4. **Signature Verification**:
    ```python
    from your_script import load_public_key
    public_key = load_public_key('public_key.pem')
    ```

## Acknowledgements

- [Cryptography](https://cryptography.io/)
- [OpenCV](https://opencv.org/)
- [Pillow](https://pillow.readthedocs.io/en/stable/)
- [PyWavelets](https://pywavelets.readthedocs.io/en/latest/)
- [TensorFlow](https://www.tensorflow.org/)
