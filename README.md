# 🎙️ VoiceXChange - AI Voice Translator

VoiceXChange is a modern, user-friendly web application that translates spoken language in real-time. It allows users to record their voice in one language and instantly get translations in multiple languages, complete with audio playback.

![VoiceXChange Demo](https://github.com/AdarshXKumAR/AI-Voice-Translator/blob/main/demo1.png)

## ✨ Features

- **Voice Recording**: Simple interface for recording your voice with visual feedback
- **Real-time Transcription**: Converts speech to text using AssemblyAI's advanced speech recognition
- **Multi-language Translation**: Supports translation between 7 languages:
  - English 🇬🇧
  - Hindi 🇮🇳
  - Japanese 🇯🇵
  - Spanish 🇪🇸
  - Russian 🇷🇺
  - German 🇩🇪
  - Korean 🇰🇷
- **Audio Playback**: Listen to both original and translated audio
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Beautiful UI**: Modern dark theme with smooth animations and visual feedback

![Translation Cards](https://github.com/AdarshXKumAR/AI-Voice-Translator/blob/main/demo2.png)

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Node.js and npm (for frontend development)
- API keys:
  - [AssemblyAI](https://www.assemblyai.com/) for speech recognition

###  Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/AdarshXKumAR/AI-Voice-Translator.git
   cd AI-Voice-Translator
   ```

2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows, use: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Create a `.env.local` file in the project root with your API keys:
   ```
   ASSEMBLYAI_API_KEY=your_assemblyai_api_key
   ```

### Running the Application

1. Start the Flask backend:
   ```bash
   python app.py
   ```

2. Open your browser and navigate to:
   ```
   http://localhost:5000
   ```

## 🛠️ Technologies Used

### Backend
- **Flask**: Lightweight web framework for Python
- **AssemblyAI API**: For accurate speech-to-text transcription
- **Google Translator**: For text translation services
- **gTTS (Google Text-to-Speech)**: For generating audio from translated text

### Frontend
- **HTML5/CSS3**: For structure and styling
- **JavaScript**: For interactive features
- **Web Audio API**: For audio recording and visualization
- **MediaRecorder API**: For capturing audio from microphone

## 📚 Project Structure

```
├── app.py                 # Flask application and API endpoints
├── static/                # Static assets
│   ├── script.js          # Frontend JavaScript
│   └── styles.css         # CSS styles
├── templates/             # HTML templates
│   └── index.html         # Main application page
├── .env.local             # Environment variables (create this file)
└── README.md              # This file
```

## 🔒 Privacy Considerations

VoiceXChange processes audio data for translation purposes:
- Audio is temporarily stored on the server during processing
- Transcription is performed through AssemblyAI's secure API
- Temporary files are automatically cleaned up after 24 hours

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgements

- [AssemblyAI](https://www.assemblyai.com/) for their speech recognition API
- [Google Translate](https://translate.google.com/) for translation services
- [Font Awesome](https://fontawesome.com/) for icons
- [Poppins](https://fonts.google.com/specimen/Poppins) font from Google Fonts

## 🚧 Future Improvements

- Add more language options
- Implement custom voice selection for each language
- Add ability to save and export translations
- Implement user accounts to save translation history
- Add offline mode with cached translations
