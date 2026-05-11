# Caesar Cipher Web Application

A modern glassmorphism-based Caesar Cipher web application built using HTML, CSS, and JavaScript.

## Features
- Encrypt text using Caesar Cipher
- Decrypt encrypted text
- Modern glassmorphism UI
- Responsive design
- Simple and user-friendly interface

## Technologies Used
- HTML
- CSS
- JavaScript

## Live Demo
https://mogudalameghana.github.io/caesar_cipher_web/

## How It Works
The Caesar Cipher shifts each alphabet letter by a fixed number of positions.

Example:
HELLO → KHOOR (Shift = 3)

## Project Purpose
This project was created to understand:
- Basic Cryptography
- Encryption & Decryption
- Web Development Concepts
- JavaScript Logic

## Sample JavaScript Logic

```javascript
function caesarCipher(text, shift) {
    let result = "";

    for (let i = 0; i < text.length; i++) {
        let char = text[i];

        if (char.match(/[a-z]/i)) {

            let code = text.charCodeAt(i);

            if (code >= 65 && code <= 90) {
                char = String.fromCharCode(
                    ((code - 65 + shift) % 26 + 26) % 26 + 65
                );
            }

            else if (code >= 97 && code <= 122) {
                char = String.fromCharCode(
                    ((code - 97 + shift) % 26 + 26) % 26 + 97
                );
            }
        }

        result += char;
    }

    return result;
}
```


## Author
Meghana Mogudala
