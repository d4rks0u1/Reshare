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
