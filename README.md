# SIH25240
AI/ML based text-to-text machine translation from Nepalese and Sinhalese to English

# Sahitya Setu (The Literature Bridge) 🌉

[](https://opensource.org/licenses/MIT)
[](https://www.google.com/search?q=./CONTRIBUTING.md)
[](https://www.python.org/downloads/)

An offline-first, AI/ML-powered platform for translating and preserving the rich literary heritage of Nepal (Nepali) and Sri Lanka (Sinhalese). This project was developed for the Smart India Hackathon (SIH) to serve organizations like the National Technical Research Organisation (NTRO).

 \#\# 📜 About The Project

A vast amount of literary and cultural heritage from Nepal and Sri Lanka remains locked in physical documents, inaccessible to a global audience. "Sahitya Setu" is designed to bridge this gap.

It's a complete ecosystem that goes beyond simple translation. It accurately digitizes complex and even handwritten documents, translates them with cultural nuance, and uses a unique human-in-the-loop system to continuously improve itself—all while working completely offline to ensure data security and privacy.

## ✨ Key Features

  * **Advanced OCR Engine:**

      * Accurately recognizes complex scripts like Devanagari (Nepali) and Sinhala.
      * Capable of digitizing **handwritten manuscripts** and historical documents.
      * Intelligently handles varied print styles and complex page layouts.

  * **Offline AI-Powered Translation:**

      * Utilizes powerful, pre-trained models (like Meta's NLLB) that run locally.
      * Focuses on preserving cultural context, idioms, honorifics, and tone.
      * Experimental "Poetry Mode" to maintain artistic integrity.

  * **Interactive Feedback Loop:**

      * A dual-pane editor allows users to compare original and translated text side-by-side.
      * Users can easily correct translations, and every correction is saved to a local SQLite database.
      * This feedback creates a valuable parallel corpus to fine-tune and improve the model over time.

  * **Rich User Experience:**

      * Export translations as `.txt` or bilingual `.pdf` files.
      * Integrated Text-to-Speech (TTS) for audio output.
      * AI-powered summarization for long documents.
      * Built-in dictionary, transliteration tools, and a personal phrasebook.

## 🛠️ Technology Stack

  * **Backend:** Python, Flask
  * **ML / AI:** Hugging Face Transformers, Tesseract OCR
  * **Database:** SQLite
  * **Frontend:** Flutter,dart
  * **Deployment:** Packaged as a standalone desktop application using PyInstaller.

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

You will need the following software installed on your system:

  * Python (3.9+) & Pip
  * Git
  * Tesseract OCR Engine
      * On Ubuntu: `sudo apt-get install tesseract-ocr`
      * On macOS: `brew install tesseract`
      * On Windows: Download from the [Tesseract installer page](https://www.google.com/search?q=https://github.com/UB-Mannheim/tesseract/wiki).
  * Tesseract language packs for Nepali (`nep`) and Sinhalese (`sin`).

### Installation

1.  **Clone the repository:**

    ```sh
    git clone https://github.com/your-username/sahitya-setu.git
    cd sahitya-setu
    ```

2.  **Create and activate a virtual environment:**

    ```sh
    # For macOS/Linux
    python3 -m venv venv
    source venv/bin/activate

    # For Windows
    python -m venv venv
    .\venv\Scripts\activate
    ```

3.  **Install the required packages:**

    ```sh
    pip install -r requirements.txt
    ```

4.  **Download ML Models:**

      * The first time you run the application, the necessary translation models from Hugging Face will be downloaded and cached automatically. Ensure you have an internet connection for this initial setup.

5.  **Run the application:**

    ```sh
    python app.py
    ```

    Navigate to `http://127.0.0.1:5000` in your web browser to use the application.



## 🙏 Acknowledgements

  * Smart India Hackathon (SIH)
  * National Technical Research Organisation (NTRO)
  * The creators of the NLLB and Tesseract projects.