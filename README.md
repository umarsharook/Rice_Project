# 🌾 Rice Type Identification AI

This project uses **Deep Learning with TensorFlow** and a **Streamlit-based web interface** to identify rice grain types from images. It supports classification of 5 rice varieties:

- Basmati
- Jasmine
- Arborio
- Glutinous
- Brown

---

## 📌 Features

- ✅ Upload and analyze rice images via a web interface
- ✅ Real-time rice type prediction with confidence scores
- ✅ Transfer learning using MobileNetV2
- ✅ Easily train your own model with custom datasets

---

## 📂 Folder Structure

```

Rice\_Identification\_Project/
├── Rice\_project.py               # Streamlit app
├── rice\_model.h5                 # Trained model
├── Raw/
│   └── training\_rice\_model.py   # Model training script
└── dataset/                      # Image dataset (used for training)
├── Basmati/
├── Jasmine/
├── Arborio/
├── Glutinous/
└── Brown/

````

---

## 🚀 Getting Started

### 🔧 Prerequisites

Make sure Python 3.7+ is installed.

Install required packages:

```bash
pip install streamlit tensorflow numpy pillow
````

---

## 🧠 Model Training

### 📁 Dataset Setup

Organize your dataset like this:

```
dataset/
├── Basmati/
│   ├── basmati1.jpg
│   └── ...
├── Jasmine/
│   ├── jasmine1.jpg
│   └── ...
├── Arborio/
├── Glutinous/
└── Brown/
```

> 📝 Each class should have 50–100+ images for better performance.

### 🔁 Train the Model

To train the model using the provided script:

```bash
python Raw/training_rice_model.py
```

This will:

* Load and preprocess the dataset
* Train using **MobileNetV2**
* Save the trained model as `rice_model.h5`

---

## 🖥️ Run the Web App

To start the Streamlit app:

```bash
streamlit run Rice_project.py
```

Then open your browser and visit:
👉 [http://localhost:8501](http://localhost:8501)

---

## 📷 Using the Application

1. Upload a rice grain image
2. Click "Predict"
3. View the rice type and confidence score

---

## 🧪 Technologies Used

* 🧠 TensorFlow / Keras
* 🖼️ MobileNetV2 (Transfer Learning)
* 🧮 NumPy
* 🖌️ Pillow (PIL)
* 🌐 Streamlit (for frontend)


## 💡 Future Improvements

* Add more rice varieties
* Improve dataset size and balance
* Deploy the app online (Streamlit Cloud, Heroku, etc.)
* Add multilingual support
* Integrate mobile camera upload

---
