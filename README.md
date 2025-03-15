# 🗣️ Speech-to-Sign-language-Translator

**An application that takes in live speech or audio recording as input, converts it into text, and displays the relevant Indian Sign Language images or GIFs.**

## ✨ Features
- **Front-end:** EasyGui
- **Speech Input:** Microphone using PyAudio
- **Speech Recognition:** Google Speech API and Sphinx (for offline use)
- **Text Preprocessing:** NLP
- **Translation:** Dictionary-based Machine Translation

## 🚀 To Run the Application
1. Open the Downloads folder and then open the terminal.
2. From the terminal, run the *main* python file using the command:
   ```sh
   python main.py
   ```
3. The application interface appears on the screen.
4. Hit the **Record** button to start taking speech as input.
5. Any speech recorded is then processed and respective outputs are shown accordingly.
6. To exit the application using speech, say **goodbye**.

## 🧏 About Sign Language
**Sign language** is a visual language that is used by deaf people as their mother tongue. Unlike acoustically conveyed sound patterns, sign language uses body language and manual communication to fluidly convey the thoughts of a person. Due to the considerable time required in learning Sign Language, it becomes difficult to communicate with these specially abled people, creating a communication gap.

## 🎯 Objective
**This Audio to Sign Language converter aims at:**
- Providing information access and services to deaf people in Indian sign language.
- Developing a scalable project which can be extended to capture the whole vocabulary of ISL through manual and non-manual signs.

It can be developed as a desktop or mobile application to enable specially abled people to communicate easily and effectively with others.

## 📜 Algorithm
### Audio to Sign Language Translator
1. **Start**
2. **Getting the Speech**
   - Listen for 1 second and calibrate the energy threshold for ambient noise levels.
   - Listen to the Speech using a Microphone.
3. **Recognize the Speech**
4. **Convert Speech to Text**
   - Make the Text lowercase for further manipulation.
5. **Detected Text**
   - If “goodbye” then exit.
   - Else if Detected Text is in predefined Dictionary Words, display respective GIFs of the Phrase.
   - Else count the letters of the Word/Phrase.
     - Display the Visual of the phrase with some delay of Actions.
   - Continue all the steps from Step 3, and continue till the Speech Ends.
6. **Error Handling**
   - If Error in Step 2, that is if no Speech is Detected, then display error message “Could not listen”.

## 🌟 Significance
The Audio to Sign Language converter is important and significant because it helps in providing information access and services to deaf people in Indian sign language. It also develops a scalable project which can be extended to capture the whole vocabulary of ISL through manual and non-manual signs. Additionally, it can be developed as a desktop or mobile application to enable specially abled people to communicate easily and effectively with others.

