# Indian Sign Language to Text Converter

A real-time web-based system that recognizes Indian Sign Language (ISL) hand gestures using Mediapipe and LSTM, converting them into readable text. This project aims to bridge the communication gap between the hearing/speech impaired and those unfamiliar with sign language.

---

## 📌 Features

- Real-time ISL hand gesture recognition
- Uses Mediapipe for hand landmark detection
- LSTM model for sequence prediction
- Converts gestures into readable text
- Web integration for live demo

---

## 📁 Project Structure

```
MP_Data/                 
├── hi how are you/
├── thank you so much/
Logs/                    
main.py                  
requirements.txt
README.md
```

## Requirements

To run the project, you need to install the following dependencies:

### ✅ `requirements.txt`

```txt
opencv-python==4.8.1.78
mediapipe==0.10.7
imutils==0.5.4
numpy==1.23.5
matplotlib==3.7.1
seaborn==0.12.2
tensorflow==2.11.0
keras==2.11.0
scikit-learn==1.2.2
```
---
## Installation

1. Clone this repository to your local machine:
  ``` bash 
   git clone https://github.com/your-username/hand-gesture-recognition.git
   cd hand-gesture-recognition
   ```
2. Install the dependencies from the requirements.txt file:
 ```bash
 pip install -r requirements.txt
  ```

## How to run?

### Step 1: Prepare the Gesture Data
Make sure the structure shoul look like this:
```bash
MP_Data/
├── hi how are you/
│   ├── 0/
│   │   ├── 0.npy
│   │   ├── 1.npy
│   ├── 1/
│   │   ├── 0.npy
│   │   ├── 1.npy
├── thank you so much/
│   ├── 0/
│   │   ├── 0.npy
│   │   ├── 1.npy


```
## Step 2: Training the Model
Now that your dataset is organized, it's time to train the model. To do this, run the following command:
 ```bash
python main.py
```

## Step 3: Start Real-Time Gesture Recognition
Once the model finishes training, it will automatically open the webcam feed. This will allow you to perform gestures in front of the camera for real-time predictions. The model will recognize the gestures and display the corresponding text output.

---

## 🖼️ Screenshots
- correct detection of the class "hello"
![image](https://github.com/user-attachments/assets/b38e7c61-1396-40ee-a2c0-9658716cbcc5)
- 📊Model Accuracy and loss during training
![WhatsApp Image 2025-03-29 at 17 51 24_c9d3a8d4](https://github.com/user-attachments/assets/26a8cd9e-9b4e-44aa-b4b7-275f1c4eb4a9)

## Troubleshooting
1. Webcam not opening or not detecting gestures: 
  Make sure your camera is properly connected and accessible.
  If you're using an external webcam, check that it is selected in your system.
  Try closing other applications that may be using the webcam.

3. Dependencies not installed:
If you encounter errors regarding missing dependencies like imutils, ensure you've installed everything with:

```bash
pip install -r requirements.txt

```

## Quitting the Webcam Feed
To stop the webcam and terminate the running process:

Press q on the webcam window.

Alternatively, you can also stop the process by pressing Ctrl + C in your terminal.

