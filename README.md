# AICTE_CyberSecurity_Project
Secure Data Hiding in Images Using Steganography is a Python-based project that utilizes Least Significant Bit (LSB) encoding to embed secret messages within images while keeping them visually unchanged. 

The project supports password protection and encryption (Fernet) for enhanced security, ensuring that only authorized users can extract the hidden data. It is implemented using Python, OpenCV, NumPy, and PIL, with compatibility for PNG, JPG, and BMP formats. 

Users can easily hide a message using hide_text("input_image.png", "Your Secret Message", "stego_image.png") and extract it with extract_text("stego_image.png"). The project is designed for cybersecurity enthusiasts, journalists, and researchers, offering future enhancements like audio/video steganography and AI-based security improvements. 

Clone the repository from GitHub, install dependencies via pip install -r requirements.txt, and start encoding messages securely! 🚀
