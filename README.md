# AICTE_CyberSecurity_Project
Secure Data Hiding in Images Using Steganography
🔒 A Python-based steganography tool that hides and extracts secret messages from images using Least Significant Bit (LSB) encoding.

📌 Features
✔ LSB Steganography: Embeds hidden messages by modifying the least significant bits of pixel values.
✔ Password Protection: Ensures only authorized users can retrieve hidden data.
✔ Encryption Support: Encrypts the message before hiding it for extra security.
✔ No Visible Changes: The encoded image looks the same as the original.
✔ Supports Multiple Formats: Works with PNG, JPG, and BMP images.

📁 Project Structure
bash
Copy
Edit
├── main.py               # Main script for encoding & decoding
├── encryption.py         # Script for optional encryption support
├── README.md             # Project documentation
├── requirements.txt      # Required dependencies
├── input_image.png       # Sample image for testing
├── stego_image.png       # Output image with hidden message

🛠️ Technologies Used
Python (Main Programming Language)
OpenCV (cv2) – Image processing
NumPy – Array manipulation
Pillow (PIL) – Image handling
Cryptography (Fernet) – Message encryption

📥 Installation
1️⃣ Clone this repository:
bash
Copy
Edit
git clone https://github.com/yourusername/secure-steganography.git
cd secure-steganography

2️⃣ Install dependencies:
bash
Copy
Edit
pip install -r requirements.txt

🔐 Usage
1️⃣ Hide a Message in an Image
python
Copy
Edit
from main import hide_text

hide_text("input_image.png", "Your Secret Message", "stego_image.png")
This will save stego_image.png with the hidden message.

2️⃣ Extract a Hidden Message
python
Copy
Edit
from main import extract_text

extract_text("stego_image.png")
This will output the extracted message.

3️⃣ (Optional) Encrypt the Message Before Hiding
python
Copy
Edit
from encryption import encrypt_message, decrypt_message

secret_msg = "This is a hidden message"
encrypted_msg = encrypt_message(secret_msg)

print("Encrypted:", encrypted_msg)
print("Decrypted:", decrypt_message(encrypted_msg))
Use the encrypted text instead of plain text for extra security.

📝 Example
Input Image

Stego Image (After Hiding Message)

Decoded Message Output
csharp
Copy
Edit
Hidden Message: This is a secret!
🚀 Future Enhancements
🔹 Support for audio and video steganography
🔹 GUI or Web Application for ease of use
🔹 AI-based detection resistance for enhanced security
🔹 Blockchain integration for tamper-proof secret storage
