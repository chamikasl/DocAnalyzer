# DocAnalyzer
Medical Prescription Analysis Tool with Chat Assistance

**DocAnalyzer** is an AI-powered medical prescription analysis tool designed to help users understand their medications better. It utilizes advanced **Optical Character Recognition (OCR)**, **Natural Language Processing (NLP)**, **Text-to-Speech (TTS)**, and **Large Language Models (LLMs)** to convert complex medical prescription details into clear, accessible insights. With DocAnalyzer, users can ask questions via an interactive chat interface, get personalized responses, and listen to prescription information through voice output.

## Table of Contents
- [Features](#features)
- [Purpose](#purpose)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Future Improvements](#future-improvements)
- [Contributing](#contributing)
- [License](#license)

## Features
- **OCR Processing**: Extracts text from medical prescription images using Google Vision API and Tesseract OCR.
- **NLP & Medical Term Recognition**: Identifies and structures key information like medication names, dosages, and instructions.
- **Interactive Chat Assistance**: Users can ask questions about their prescriptions and get real-time, context-aware responses.
- **Text-to-Speech (TTS)**: Converts text-based prescription information into audio, improving accessibility for visually impaired users.
- **User-Friendly Interface**: Simple, responsive design making it easy for anyone to upload and analyze prescriptions.

## Purpose
The primary goal of DocAnalyzer is to empower users by making medical information more accessible and understandable. The tool aims to:
- Help users better understand their medications, including usage instructions and possible side effects.
- Support visually impaired users by providing a voice output for their prescriptions.
- Assist healthcare providers in offering patients an easy way to understand their medication details.

## Technologies Used
- **Backend**: Python, Flask
- **Optical Character Recognition (OCR)**: Google Vision API, Tesseract OCR
- **Natural Language Processing (NLP)**: Spacy, OpenAI API for LLMs
- **Text-to-Speech (TTS)**: gTTS
- **Frontend**: HTML, CSS, JavaScript
- **Data Storage**: PostgreSQL (optional for deployment)
- **Other**: Trello (for project management)

## Installation
### Prerequisites
- Python 3.8+
- Google Cloud account for Vision API
- OpenAI API key
- PostgreSQL (optional)

### Setup
1. **Clone the repository**:
   git clone https://github.com/yourusername/DocAnalyzer.git
   cd DocAnalyzer
   Create and activate a virtual environment:
2. **Create and activate a virtual environment**:
   python3 -m venv venv
   source venv/bin/activate
3. **Install dependencies**:
   pip install -r requirements.txt
4. **Set up environment variables**:
   Create a .env file in the root directory and add the following keys:
   GOOGLE_API_KEY="your_google_api_key"
   OPENAI_API_KEY="your_openai_api_key"
5. **Run the application**:
   flask run
6. **Access the app**:
   Open your browser and go to http://localhost:5000.

## Usage
- **Upload Prescription**: Users can upload an image of their prescription.
- **Text Extraction and Analysis**: DocAnalyzer extracts text from the image and identifies important medical details using NLP and LLMs.
- **Ask Questions**: Through the chat interface, users can ask questions about their prescription.
- **Listen to Prescription Details**: For visually impaired users or those who prefer audio, DocAnalyzer can read out the prescription details using TTS.

## Project Structure

    DocAnalyzer/
    ├── app/                   
    │   ├── static/            # CSS, JavaScript, images
    │   ├── templates/         # HTML templates
    │   ├── modules/           # Core modules (OCR, NLP, Chat, TTS)
    │   ├── __init__.py        # App setup
    │   ├── config.py          # Configurations and environment settings
    │   ├── routes.py          # App routes
    │   ├── utils.py           # Helper functions
    ├── requirements.txt       # Required packages
    ├── README.md              # Project documentation
    └── .env                   # Environment variables (Google API Key, OpenAI API Key)
    
## Future Improvements
- **Handwriting Recognition**: Enhance OCR capabilities to better recognize handwritten prescriptions.
- **Multilingual Support**: Expand language support for a wider user base.
- **Real-Time Data Integration**: Integrate with live medical databases for real-time drug information.
- **Mobile App**: Develop a mobile version for on-the-go use.
  
## Contributing
Contributions are welcome! Please fork the repository, create a feature branch, and submit a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.
