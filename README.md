# 🌾 CropCast

**CropCast** is an AI-powered **crop recommendation system** that uses machine learning to suggest the most suitable crop based on soil and environmental parameters.  
It is built with **Flask** for the backend and a clean **HTML interface** for user interaction — designed to assist farmers and researchers in making data-driven agricultural decisions.

---

## 🚀 Overview

CropCast analyzes the following agricultural parameters:
- **Nitrogen (N)**
- **Phosphorus (P)**
- **Potassium (K)**
- **Temperature**
- **Humidity**
- **pH**
- **Rainfall**

Based on these inputs, it predicts the **best crop** suited for the given conditions.  
The prediction model is trained using the `Crop_recommendation.csv` dataset and integrated into the Flask web app.

---

## 🎯 Features

- 🌱 Predicts optimal crop recommendations.
- 🧠 Uses a trained ML model (`model.pkl`) built on real-world data.
- 💻 Interactive and lightweight Flask web interface.
- 🔄 Automatically resets output when the page is refreshed.
- 🗂 Organized project structure with clear separation of concerns.

---

## 🧩 Tech Stack

| Layer | Technology |
|:------|:------------|
| **Frontend** | HTML, CSS (Flask Templates) |
| **Backend** | Python, Flask |
| **Machine Learning** | scikit-learn, NumPy, Pandas |
| **Dataset** | Crop Recommendation Dataset (`Crop_recommendation.csv`) |

---

## 📂 Project Structure
```
CropCast/
│
├── app.py # Main Flask application
├── model.pkl # Trained ML model (serialized with pickle)
├── model.ipynb # Jupyter Notebook for model training
├── Crop_recommendation.csv # Dataset used for training
│
├── templates/
│ └── index.html # Frontend HTML template
│
└── static/
└── style.css # CSS styling
```

---

## ⚙️ Installation & Setup

### Prerequisites
Make sure you have the following installed:
- Python 3.9 or higher  
- pip (Python package manager)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/ShishirSuman999/CropCast.git
   cd CropCast
2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
3. **Run the Flask app**
   ```bash
   python app.py
4. **Open in browser**
   ```bash
   http://127.0.0.1:5000/

---

## 🔍 How It Works

- User enters environmental and soil parameters (N, P, K, etc.) into the form.
- The data is processed and converted into a NumPy array.
- The trained ML model (model.pkl) predicts the most suitable crop.
- The result is displayed dynamically on the web page.

---

##  🤝 Contributions

### Contributions are always welcome!
Here’s how you can help improve CropCast:
- Fork the repository
- Create a new branch (git checkout -b feature-name)
- Commit your changes (git commit -m "Added new feature")
- Push to your branch (git push origin feature-name)
- Open a Pull Request

Possible areas of improvement:
- Adding more crops or updated datasets
- Enhancing the UI/UX
- Improving model accuracy
- Integrating real-time weather data APIs
