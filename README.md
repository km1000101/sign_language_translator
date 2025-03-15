Speech-to-Sign-Language Translator 🗣️🤟
  

A desktop application that converts live speech or audio recordings into text and displays corresponding Indian Sign Language (ISL) images or GIFs, fostering communication with the deaf community.

🌟 Overview
Sign language is a vital communication tool for the deaf community, relying on visual gestures and body language instead of spoken words. Learning sign language can be challenging and time-intensive, often creating barriers between hearing and deaf individuals. This project bridges that gap by converting spoken language into Indian Sign Language (ISL) visuals in real-time.

Key Features
🎙️ Speech Input: Accepts live speech via microphone or pre-recorded audio.
📝 Speech-to-Text: Uses Google Speech API (online) or CMU Sphinx (offline) for speech recognition.
✍️ Text Preprocessing: Processes text with NLP for accurate translation.
🤟 Sign Language Translation: Converts text into ISL images or GIFs using a dictionary-based approach.
🖥️ User Interface: Built with EasyGui for simplicity and ease of use.
📈 Scalable Design: Extensible to include the full ISL vocabulary with manual and non-manual signs.
🎯 Objective
The Speech-to-Sign-Language Translator aims to:

Provide accessible communication tools for deaf individuals using Indian Sign Language.
Develop a scalable solution to eventually encompass the entire ISL vocabulary.
Enable seamless interaction between hearing and deaf individuals via a desktop or mobile app.
🚀 Getting Started
Prerequisites
Ensure the following are installed on your system:

Python 3.x
Dependencies:
PyAudio (audio input)
SpeechRecognition (speech-to-text)
EasyGui (GUI)
NLTK or spaCy (NLP text preprocessing)
CMU Sphinx (optional, for offline speech recognition)
A working microphone for live speech input.
A dataset of ISL images or GIFs mapped to words/phrases.
Install dependencies:

bash

Collapse

Wrap

Copy
pip install pyaudio speechrecognition easygui nltk
Installation
Clone or download this repository:
bash

Collapse

Wrap

Copy
git clone https://github.com/yourusername/speech-to-sign-language-translator.git
Navigate to the project directory:
bash

Collapse

Wrap

Copy
cd speech-to-sign-language-translator
Run the application:
bash

Collapse

Wrap

Copy
python main.py
Usage
Launch the application to open the EasyGui interface.
Click the "Record" button to start capturing speech.
Speak clearly into your microphone.
The app will convert your speech to text and display the corresponding ISL visuals.
Say "goodbye" to exit the application.
🛠️ How It Works
The application follows these steps:

Initialize: Calibrates the microphone for ambient noise.
Capture Speech: Records audio using PyAudio.
Recognize Speech: Converts audio to text using Google Speech API or CMU Sphinx.
Preprocess Text: Converts text to lowercase and processes it with NLP.
Translate to ISL:
Matches text with dictionary entries to display ISL GIFs/images.
If no match, breaks text into words/letters and shows visuals sequentially.
Error Handling: Displays "Could not listen" if no speech is detected.
Loop: Continues until the user says "goodbye."
📂 Project Structure
text

Collapse

Wrap

Copy
speech-to-sign-language-translator/
│
├── main.py                 # Main script to run the app
├── speech_processing.py    # Handles speech capture and recognition
├── text_processing.py      # Preprocesses text using NLP
├── translation.py          # Converts text to ISL visuals
├── assets/                 # Directory for ISL images/GIFs
│   ├── hello.gif
│   ├── goodbye.gif
│   └── ...
├── dictionary.json         # Maps words/phrases to ISL visuals
└── README.md               # Project documentation
🔮 Future Enhancements
Expand the ISL dictionary to cover the full vocabulary.
Support non-manual signs (e.g., facial expressions).
Generate real-time ISL videos using machine learning.
Develop a mobile app for broader accessibility.
Add multilingual support for wider usability.
⚠️ Limitations
Requires an internet connection for Google Speech API (unless using Sphinx offline).
Limited to the predefined ISL dictionary.
Accuracy depends on speech clarity and microphone quality.
🤝 Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a new branch (git checkout -b feature-branch).
Make your changes and commit (git commit -m "Add feature").
Push to the branch (git push origin feature-branch).
Create a pull request.
Areas for contribution:

Adding more ISL visuals to the dictionary.
Improving speech recognition in noisy environments.
Enhancing the UI for better accessibility.
📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

🙏 Acknowledgments
The deaf community for inspiring this project.
Open-source libraries: SpeechRecognition, PyAudio, EasyGui.
Contributors and supporters who help improve this project.
By enabling communication through Indian Sign Language, this project fosters inclusivity and bridges the gap between hearing and deaf individuals. Let's make communication accessible for everyone! 💬🤟
