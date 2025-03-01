# ऋ Share v1
## Overview

This app is designed to enable seamless file sharing over a local network using Wi-Fi or a mobile hotspot. The system eliminates the need for cables, Bluetooth, or cloud uploads, allowing users to transfer files at high speeds directly between devices, from pc to any mobile device which has hotspot.
## Features

- Web Interface: Provides an easy-to-use dashboard for uploading and downloading files.
- Hotspot Enabled: Works without Wi-Fi by turning one device into a hotspot.
- Upload any file type via a simple web interface.
- View uploaded files with timestamps.
- Download files with a single click.
- Fully offline, no external dependencies.
- Built with Flask and local resources.
- Start the application easily using `start.bat` (Windows) or `python app.py` (Linux)


## Installation

### Prerequisites

- Python 3.x installed
- Flask installed (`pip install flask`)

### Clone the Repository

```sh
git clone https://github.com/d4rks0u1/Reshare
cd Reshare
```

### Run the App

```sh
python app.py
```

The application will run on `http://0.0.0.0:80`.

## File Structure

```
project-root/
│-- app.py  # Main Flask application
│-- templates/
│   │-- index.html  # Homepage
│   │-- send.html  # Upload page
│   │-- files.html  # Files listing page
│   │-- upload/  # Directory where uploaded files are stored
│-- static/
│   │-- uploader.js  # Local file upload script
│   │-- styles.css  # Custom styles
│-- README.md  # User guide
```

## Usage


## **Running the Application**
### **For Windows**
1. Navigate to the project directory.
2. Double-click `start.bat` or run the following command in Command Prompt:
   ```batch
   start.bat
   ```

### **For Linux**
1. Open a terminal in the project directory.
2. Run the following command:
   ```bash
   python3 app.py
   ```

## **Usage**
1. Open the browser and navigate to:
   ```
   http://localhost
   ```
   or check the console output for the IPv4 address to access it from another device on the same network.
2. Use the "Upload" section to select and upload a file.
3. Go to the "Files" section to view or download uploaded files.
4. Click the "⬅ Go Back" button to return to the home page.

## **Dashboard IPv4 Display Feature**
- The application will display a link with the system’s local IPv4 address.
- You can use this link to access the dashboard from other devices on the same network.

## **Stopping the Application**
- On Windows: Close the command prompt window.
- On Linux: Press `CTRL + C` in the terminal.

## **Troubleshooting**
- **Issue**: Flask is not installed.
  **Solution**: Run `pip install flask`.
- **Issue**: Port 80 is already in use.
  **Solution**: Modify `app.run(host='0.0.0.0', port=80, debug=True)` in `app.py` to use another port, e.g., `port=5000`.

### Upload a File

1. Open `http://localhost` in your browser.
2. Click on "Upload File".
3. Select a file and upload it.

### View & Download Files

1. Navigate to the files page.
2. Click on a file to download it.

## Customization

- Modify `styles.css` for UI changes.
- Change the upload directory in `app.py` by updating `UPLOAD_FOLDER`.
