
# 💵 Currency Note Classification Using Deep Learning

This project classifies Bangladeshi currency notes using a Convolutional Neural Network (CNN) model. The model can identify currency denominations from images (1, 2, 5, 10, 20, 50, 100, 500, and 1000 Taka).

---

## 📌 Project Objective

To develop a deep learning model that can accurately classify Bangladeshi currency notes using image input, and deploy it on a web platform (Flask/Streamlit) to take user input and return real-time predictions.

---

## 🛠 Tools & Technologies

- Python 3.10+
- TensorFlow / Keras
- OpenCV
- NumPy
- Matplotlib
- Google Colab (for training)
- Flask / Streamlit (for deployment)
- HTML, JS (for front-end integration)

---

## 🧱 Project Structure

Currency-Note-Classification/
│
├── dataset/
│   └── [images of currency notes]
├── src/
│   ├── train.py            # Model training
│   ├── model.h5            # Trained CNN model
│   ├── predict.py          # Prediction logic
│   └── app.py              # Flask web app
├── flowchart.png           # Project workflow
├── presentation_slide.pptx # Presentation
├── demo_video.mp4          # Short video demo
├── project_proposal.pdf    # Project plan
├── requirements.txt        # Libraries
└── README.md               # This file

---

## 📈 How It Works – Step by Step

### Step 1: 🖼️ Data Collection
- Images of 7 denominations collected (10–1000 Taka).
- Each category contains ~100+ labeled images.

### Step 2: ⚙️ Preprocessing
- Images resized to 224x224 pixels.
- Normalization done (divided pixel values by 255).
- Augmentation applied (rotation, zoom, flip).

### Step 3: 🧠 Model Training
- Built a CNN using Keras.
- Used Conv2D, MaxPooling2D, Dropout, Dense layers.
- Trained on 80% data; tested on 20%.
- Achieved 90–92% accuracy.

### Step 4: 📦 Saving the Model
- Final model saved as `model.h5` for deployment.

### Step 5: 🚀 Deployment (Flask / Streamlit)
- Created a web app (`app.py`) using Flask.
- Users can upload images via browser.
- Model loads and returns the predicted note.

---

## 🔧 Dependencies / Required Libraries

All required libraries are listed in `requirements.txt`. Install with:

pip install -r requirements.txt

**Key Libraries:**
- `tensorflow`
- `keras`
- `opencv-python`
- `flask` *(for Flask version)*
- `streamlit` *(for Streamlit version)*

---

## 🧪 Sample Output

| Sample Image           | Predicted Label  |
|------------------------|------------------|
| 100_taka.jpg           | 100 Taka         |
| 500_taka.jpg           | 500 Taka         |

---

## 🔮 Future Improvements

- Add fake note / counterfeit detection
- Real-time webcam capture
- Mobile App version (Android/iOS)
- Voice output (for blind users)
- Larger dataset for better accuracy

---

## 👨‍💻 Contributors

- **Bayzid Mostak** – ID: 210303020010  
- **Amith Ghosh** – ID: 210303020001  
Dept. of CSE, 8th Semester, NEUB

---
