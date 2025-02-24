# Visiting_Card_Extraction_Powered_By_OCR_NER

# Visiting Card Extraction

## Project Overview
This project is a **Visiting Card Extraction System** that leverages **Named Entity Recognition (NER)** to extract structured information from business cards. It uses **Deep Learning (NER-VC_model.h5)** for text recognition and **Flask** for the web-based interface.

The system processes visiting card images to extract key details like:
- Name
- Designation
- Company Name
- Contact Number
- Email Address
- Website URL
- Address

## Features
- **Upload visiting card images** for automatic extraction.
- **Named Entity Recognition (NER)** model to recognize text fields.
- **Web-based interface** for a seamless user experience.
- **Stores extracted information** in a structured format.
- **User-friendly UI** for easy interaction.
- **Supports different visiting card formats** and image resolutions.

## Tech Stack
### Backend
- **Python 3.x**
- **Flask** (Web framework)
- **TensorFlow/Keras** (Deep Learning for NER)
- **Pandas & NumPy** (Data processing)
- **OpenCV & Tesseract OCR** (Image Processing)

### Frontend
- **HTML, CSS, JavaScript** (for UI)
- **Bootstrap** (Responsive design)

### Data Storage
- **CSV / SQLite** (For storing extracted data)

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- **Python 3.x**
- **Flask**
- **TensorFlow / Keras**
- **Tesseract OCR** (for text extraction)

### Steps to Setup
1. Clone or extract the repository:
   ```sh
   git clone https://github.com/your-repo/Visiting_Card_extraction.git
   cd Visiting_Card_extraction
   ```
2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Install **Tesseract OCR** (if not installed):
   - **Windows:** Download and install from [Tesseract GitHub](https://github.com/tesseract-ocr/tesseract)
   - **Linux:** Install via package manager:
     ```sh
     sudo apt install tesseract-ocr
     ```
4. Run the Flask application:
   ```sh
   python app.py
   ```
5. Open your browser and visit:
   ```
   http://127.0.0.1:5000/
   ```

## Folder Structure
```
Visiting_Card_extraction/
│── app.py                # Main Flask application
│── Dataset.csv           # Dataset for model training
│── NER-VC_model.h5       # Pre-trained NER model
│── requirements.txt      # Required dependencies
│── static/               # Static assets (CSS, JS, images)
│── templates/            # HTML templates for UI
│── uploads/              # Folder for uploaded images
```

## Usage
1. **Upload a visiting card image** via the web interface.
2. The system processes the image and extracts relevant information.
3. **Extracted details** are displayed on the web UI.
4. Option to **save extracted data** in CSV/Database.

## Model Details
- The **NER model** is trained using a dataset of business card text fields.
- **TensorFlow/Keras** is used for deep learning-based entity recognition.
- **OCR (Tesseract & OpenCV)** is used for image-to-text conversion.

## Future Improvements
- **Enhance OCR accuracy** using advanced deep learning models.
- **Integrate database storage** (SQLite or MongoDB).
- **Enable multi-language support**.
- **Automate data correction** for inaccurate text extraction.
- **Mobile app integration** for real-time scanning.
- **Integration of the project with a contact app**

## Troubleshooting
**Issue:** Model not recognizing text accurately?
- Ensure **Tesseract OCR** is installed properly.
- Use **high-quality images** with clear text.

**Issue:** Flask app not starting?
- Check if **Python and Flask** are installed correctly.
- Run `pip install -r requirements.txt` to install dependencies.


