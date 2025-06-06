# 🧠 REAl TIME ISL TO TEXT 

A two-feature application designed to improve communication for people with hearing and speech impairments using advanced speech processing and computer vision techniques.

---

## 📌 Features

### 🔹 Feature 1: Action Detection in Real-Time (Using Computer Vision)

**Description:**
A real-time action detection module that captures and classifies user actions via webcam using pose estimation and machine learning techniques.

**Technologies Used:**
- Python
- OpenCV
- MediaPipe (Pose Estimation)
- scikit-learn (for action classification)
- NumPy and Matplotlib

**Working Steps:**
1. Capture live video feed using webcam.
2. Detect body pose using MediaPipe.
3. Extract keypoints and track movement.
4. Use a trained model to classify the detected actions (e.g., waving, pointing, etc.).
5. Display the predicted action in real-time on the screen.

**Use Case:**
- Can be used for gesture-based input in interactive systems.
- Helps recognize physical intent in absence of speech.

---

### 🔹 Feature 2: Speech-to-Sign-language Translator

**Description:**
An application that takes live speech or audio recording as input, converts it into text, and displays the relevant Indian Sign Language (ISL) signs as images or GIFs.

**Technologies Used:**
- Python
- EasyGui (Frontend GUI)
- PyAudio (Microphone input)
- Google Speech API & CMU Sphinx (Speech Recognition)
- NLP (Text preprocessing)
- Dictionary-based translation
- Custom ISL Dataset (GIFs and images)

**Preprocessing:**
- Convert speech to lowercase text.
- Remove punctuation and extra whitespace.
- Tokenize and map words to ISL GIFs.
- If no match found, fallback to ISL alphabet spelling.

**Dataset:**
- Custom curated Indian Sign Language dataset.
- Includes signs for alphabets and commonly used words/phrases.

**How It Works:**
1. User speaks into the mic.
2. Speech is converted to text.
3. Text is preprocessed and compared with dictionary.
4. Corresponding ISL GIFs are shown as output.
5. If “goodbye” is said, the app exits.

---

## 🚀 Installation & Usage

### 🔧 Requirements
- Python 3.7+
- `opencv-python`
- `mediapipe`
- `pyaudio`
- `speechrecognition`
- `easygui`
- `scikit-learn`
- `matplotlib`
- `numpy`

Install dependencies using:
```bash
pip install -r requirements.txt
```

### ▶️ Running Feature 1
```bash
python action_detection.py
```

### ▶️ Running Feature 2
```bash
python main.py
```

---

## 🧑‍💻 Authors
- [Your Name]
- [Your Collaborators]

---

## 📃 License
This project is open-source and available under the [MIT License](LICENSE).

---

## 📸 Screenshots or Demo (Optional)
_Add demo images or GIFs for both features here to show functionality visually._

---

## 🌟 Future Scope
- Add full vocabulary coverage for ISL.
- Implement continuous action tracking in Feature 1.
- Create mobile version for broader accessibility.

---

