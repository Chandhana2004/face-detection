# 👁️ Face Detection using OpenCV

This project performs **real-time face detection** using a webcam feed.  
It uses **OpenCV's Haar Cascade classifier**, a pre-trained deep learning model designed to quickly detect human faces in live video streams.

---

## 🚀 Features

- Real-time face detection using webcam  
- Uses Haar Cascade (pre-trained face detection model)  
- Lightweight and fast  
- Runs entirely on CPU  
- Beginner-friendly implementation  

---

## 🛠️ Technologies Used

- **Python 3.11**
- **OpenCV (cv2)**
- Haar Cascade Classifier

---

## 📂 Project Structure

Face-Detection/
│── face_detection.py
│── README.md

---

## 📦 Installation

Install required library:

bash
pip install opencv-python

▶️ How to Run

1.Clone or download this repository.

2.Open the folder in Terminal or CMD.

3.Run:
python face_detection.py

4.Your webcam will open and detect faces in real-time.

5.Press ESC to exit.

📸 How It Works (Simple Explanation)

1.OpenCV captures frames from the webcam.

2.Each frame is converted to grayscale.

3.Haar Cascade scans the image and detects faces.

4.A rectangle is drawn around every detected face.

5.Updated frames are shown live on the screen.

🧠 Code Overview

face = cv2.CascadeClassifier(cv2.data.haarcascades + "haarcascade_frontalface_default.xml")

cap = cv2.VideoCapture(0)

Loads pre-trained face detection model

Opens the webcam

gray = cv2.cvtColor(frame, cv2.COLOR_BGR2GRAY)

faces = face.detectMultiScale(gray, 1.3, 5)

Converts to grayscale

Detects faces at different scales

cv2.rectangle(frame, (x, y), (x+w, y+h), (255, 0, 0), 2)

Draws a blue bounding box around every detected face

🧪 Example Output

- Blue rectangle around detected face(s)

- Smooth real-time performance

📚 Future Improvements

- Add eye detection

- Add smile detection

- Replace Haar Cascade with a deep learning model

- Add face recognition (identify person)

🤝 Contributing

Pull requests are welcome!

📜 License

This project is open-source and available under the MIT License.
