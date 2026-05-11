# Caesar Cipher Web Application

A                                                                                                                                                                                                 Caesar Cipher web application developed using HTML, CSS, and JavaScript.

This project helped me understand the fundamentals of cryptography, encryption techniques, front-end web development, and JavaScript logic implementation. I designed and developed the complete interface and functionality while exploring how classical encryption algorithms work in real-world cybersecurity concepts.

---

## Features

- Encrypt text using Caesar Cipher Algorithm
- Decrypt encrypted messages
- Modern Glassmorphism User Interface
- Responsive and interactive design
- User-friendly web application
- Real-time encryption and decryption

---

## Technologies Used

- HTML
- CSS
- JavaScript
- GitHub Pages

---

## Live Demo

https://mogudalameghana.github.io/caesar_cipher_web/

---

## What I Learned

Through this project, I learned:

- Basics of Cryptography
- Caesar Cipher Encryption Technique
- Encryption and Decryption Logic
- ASCII Character Manipulation
- JavaScript DOM Manipulation
- Front-End UI Design
- Glassmorphism Styling
- GitHub Repository Management
- GitHub Pages Deployment

This project improved my problem-solving skills and helped me understand how simple encryption techniques can be implemented in web applications.

---

## Challenges Faced

While building this project, I faced several challenges such as:

- Understanding character shifting logic
- Handling uppercase and lowercase letters separately
- Designing a modern responsive UI
- Deploying the project using GitHub Pages
- Fixing file naming and hosting issues

By solving these issues, I gained practical experience and confidence in both development and deployment.

---

## Sample JavaScript Logic

```javascript
function caesarCipher(text, shift){

    let result = "";

    for(let i = 0; i < text.length; i++){

        let char = text[i];

        if(char.match(/[a-z]/i)){

            let code = text.charCodeAt(i);

            if(code >= 65 && code <= 90){

                char = String.fromCharCode(
                    ((code - 65 + shift) % 26 + 26) % 26 + 65
                );
            }

            else if(code >= 97 && code <= 122){

                char = String.fromCharCode(
                    ((code - 97 + shift) % 26 + 26) % 26 + 97
                );
            }
        }

        result += char;
    }

    return result;
}
## Project Purpose
This project was created to understand:
- Basic Cryptography
- Encryption & Decryption
- Web Development Concepts
- JavaScript Logic

## Author
Meghana Mogudala
