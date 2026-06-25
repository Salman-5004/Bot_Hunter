# Bot_Hunter
Deep Fake voice detection on the basis of breath pause , pitch perfection and background noise data

BotHunter is an AI-powered Deepfake Audio Detection system designed to distinguish between genuine human voices and AI-generated (deepfake) voices based on forensic audio features.

The system analyzes characteristics such as:

* Breath pauses per minute
* Pitch perfection score
* Background noise consistency

A machine learning model processes these features and predicts whether the input voice is **Human** or **Deepfake**.

---

## Features

* Detects AI-generated voice clones.
* Uses Machine Learning for classification.
* Interactive web interface built with Gradio.
* Displays prediction confidence scores.
* Lightweight and easy to deploy.

---

## Project Structure

```text
BotHunter/
│
├── app.py                 # Main application
├── model.pkl              # Trained ML model
├── requirements.txt       # Required Python libraries
├── README.md              # Project documentation
└── dataset/               # Dataset used for training
```

---

## Technologies Used

* Python
* Scikit-learn
* Gradio
* NumPy
* Pandas

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/BotHunter.git
cd BotHunter
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Application

Execute the following command:

```bash
python app.py
```

After running the script, Gradio will generate a local URL similar to:

```text
http://127.0.0.1:7860
```

Open the URL in your browser to access the application.

---

## Input Parameters

| Feature                      | Description                                                                                          |
| ---------------------------- | ---------------------------------------------------------------------------------------------------- |
| Breath Pauses                | Number of breathing pauses per minute.                                                               |
| Pitch Perfection Score       | Indicates how smooth and consistent the pitch is. AI voices often have highly stable pitch patterns. |
| Background Noise Consistency | Measures the consistency of background noise present in the audio.                                   |

---

## Model Prediction

The model classifies audio into one of the following categories:

* **HUMAN VERIFIED** ✅
* **DEEPFAKE DETECTED** 🚨

Additionally, the system provides a confidence score for each prediction.

---

## Example Output

```text
🚨 SYSTEM ALERT: DEEPFAKE DETECTED!
Confidence: 97.45%
```

or

```text
✅ HUMAN VERIFIED.
Confidence: 94.12%
```

---

## Future Improvements

* Automatic extraction of audio features from uploaded audio files.
* Integration of MFCC, jitter, shimmer, and spectral features.
* Support for real-time audio detection.
* Deep Learning-based detection models.
* Deployment on cloud platforms.

---

## Authors

Developed as a Machine Learning and Cybersecurity project.

---

## License

This project is intended for educational and research purposes.
