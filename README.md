Face Scan Attendance System
Welcome to the Face Scan Attendance System, an advanced Python-based solution for automated attendance tracking using facial recognition. This system captures and encrypts face data securely, recognizes individuals in real-time, and logs their attendance in an Excel sheet with timestamps. Ideal for offices, schools, or any organization looking to modernize attendance management.

Developed by Aakash, this project combines AI-driven face recognition with robust encryption to ensure privacy and efficiency.

Features
Secure Face Recognition: Uses face_recognition library to generate and compare 128D face encodings.

Data Encryption: Encrypts face data with AES-256 using the cryptography library to protect user privacy.

Automated Attendance: Marks "Present" in a daily Excel sheet with user ID and timestamp upon recognition.

Real-Time Processing: Scans faces via webcam and provides instant feedback.

Scalable Design: Supports multiple users and can be extended for commercial applications.

Prerequisites
Python 3.x installed on your system.

A webcam for capturing face data.

Basic familiarity with running Python scripts and installing dependencies.

Installation
Clone this repository to your local machine:

bash
git clone https://github.com/aaka8h-bot/face-scan.git
cd face-scan
Install the required libraries using pip:

bash
pip install opencv-python face_recognition cryptography openpyxl
Create necessary directories for storing data:

encodings/ for encrypted face data.

attendance/ for Excel attendance sheets.
Run the following commands to create them:

bash
mkdir encodings attendance
Usage
Register a User:

Run the script and select 'r' for registration mode.

Enter a unique user ID (e.g., employee001).

Look at the webcam to capture your face. The system will encrypt and save your data.

bash
python face_scan.py
Mark Attendance:

Run the script and select 'a' for attendance mode.

Look at the webcam. If recognized, your attendance will be marked in an Excel file under attendance/ with the current date.

View Attendance:

Open the Excel file (e.g., attendance_2025-07-27.xlsx) in the attendance/ folder to see records with columns: User ID, Status, and Timestamp.

Quit Webcam:

Press 'q' while the webcam window is active to close it.

Security Notes
Face encodings are encrypted using a secure key stored in secret.key. Protect this key to prevent unauthorized access to data.

If the key is lost, encrypted data cannot be decrypted. Consider using a key management system for production environments.

Potential Applications & Monetization
This system can be adapted for commercial use:

Deploy as a SaaS product for businesses or educational institutions in India.

Integrate with cloud storage for remote access and charge per user or per organization.

Offer customization services for specific client needs (e.g., multi-face recognition, web interfaces).

Contact
For inquiries, support, or collaboration opportunities, reach out to the project owner:

Aakash

Telegram: t.me/aaka8h

License
This project is open-source and available for personal and commercial use. Please contact the owner for specific licensing terms if you plan to monetize or redistribute.

Thank you for checking out the Face Scan Attendance System! If you find this project useful, consider contributing or reaching out for potential partnerships.
