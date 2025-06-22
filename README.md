# Speech Emotion Recognition using CNN

This project implements a **Speech Emotion Recognition (SER)** system using **MFCC features** and a **Convolutional Neural Network (CNN)**. The model can classify audio clips into emotions such as *neutral*, *calm*, *happy*, *sad*, *angry*, *fearful*, *disgust*, and *surprised*.

---

## 🚀 Features
- Extracts MFCC features from `.wav` audio files.
- Supports both speech and song datasets.
- Visualizes emotion distribution, audio duration, and MFCCs.
- Builds and trains a CNN with dropout and early stopping.
- Evaluates using accuracy, F1 score, confusion matrix, and classification report.
- Allows emotion prediction from a custom audio file.

---

## 📂 Dataset
This project uses audio files located at:
- `Audio_Speech_Actors_01-24`
- `Audio_Song_Actors_01-24`

Each file is named using a convention that encodes the emotion label.

---

## 📌 Requirements

Install the required packages:
```bash
pip install numpy pandas librosa seaborn matplotlib scikit-learn keras tensorflow
````

---

## 🛠 How to Run

1️⃣ Update the paths for your audio datasets:


```python
speech_path = r"C:\Desktop\Audio_Speech_Actors_01-24"
song_path = r"C:\Desktop\Audio_Song_Actors_01-24"
```

2️⃣ Run the script:

```bash
python your_script.py
```

3️⃣ After training, you can test with a custom `.wav` file:

```bash
Enter full path of .wav audio file:
```

---

## 📊 Outputs

* Emotion distribution plots
* Audio duration histograms
* MFCC heatmaps
* Training/validation accuracy & loss plots
* Confusion matrix
* Classification report

---

## 🧠 Model Architecture

* `Conv2D` layers + `MaxPooling2D`
* `Flatten` + `Dense` layers
* `Dropout` regularization
* `Softmax` output for multi-class classification

---

## 💡 Example command for prediction

After model trains:

```
Enter full path of .wav audio file: C:\Desktop\test_audio.wav
Predicted Emotion: happy
```

---

## ⚠ Notes

* Ensure all `.wav` files are valid and readable by `librosa`.
* Files shorter than 3 seconds will be zero-padded.

---

## 📌 License

This project is provided for educational purposes.
