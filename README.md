# Certificate_generator
Certificate Generator with QR Code  This Python script automates the creation of personalized certificates with embedded QR codes, using data from an Excel file. It generates PDF certificates with recipient details and event information, making it ideal for efficiently managing digital certificates for events and workshops.


**Certificate Generator with Embedded QR Code**
Overview
This project automates the creation of certificates with embedded QR codes using data from an Excel file. The generated certificates are saved as PDF files, with the recipient's name, event details, and the event date included on each certificate.

**Features**
QR Code Generation: Automatically generates a QR code containing the recipient's name, event name, and event date.
Certificate Generation: Creates certificates using a background image, recipient details, and the generated QR code.
Excel Integration: Reads recipient data from an Excel file to automate the certificate creation process.
Prerequisites

**Make sure you have the following installed:**
Python 3.x
openpyxl library for reading Excel files
Pillow library for image manipulation
qrcode library for generating QR codes
You can install the required libraries using pip:
pip install openpyxl pillow qrcode[pil]

**Project Structure**
background.jpg: The background image for the certificates. Place this image in the project directory.
Participant_Data.xlsx: The Excel file containing participant data. Each row should have the recipient's name, event name, and event date.
F1/: Directory where the generated certificates are saved as PDF files.
Usage

**Prepare the Excel File:**

Create an Excel file (Participant_Data.xlsx) with the following columns:
Recipient Name (Column A)
Event Name (Column B)
Certificate Date (Column C)
Add Background Image:

Ensure a background image named background.jpg is placed in the same directory as the script.
Run the Script:

Execute the script by running the following command:
python your_script_name.py
The script will read the data from the Excel file, generate the certificates with embedded QR codes, and save them as PDF files in the F1/ directory.

Customization
Font Styles:

You can customize the fonts used for text on the certificates by modifying the paths to the font files and changing the font sizes in the script.
Certificate Layout:

The positions of text and the QR code on the certificate can be adjusted by modifying the coordinates in the script.
Error Handling
Missing Files:

The script checks if the background.jpg and Participant_Data.xlsx files are present. If not, an error message is displayed.
Invalid Date:

The script only processes rows where the Certificate Date is a valid datetime object.
