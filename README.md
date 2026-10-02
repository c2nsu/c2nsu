<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F172A,100:2563EB&height=220&section=header&text=Sakine%20Cansu%20Topci&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=35&desc=Aspiring%20Data%20Analyst%20%7C%20Web%20Developer%20%7C%20AI%20Enthusiast&descAlignY=55&descSize=18"/>
</p>

<h1 align="center">Hi 👋 I'm Sakine Cansu Topci</h1>

<h3 align="center">
Management Information Systems Graduate
</h3>

<p align="center">
📊 Aspiring Data Analyst • 💻 Web Developer • 🤖 AI Enthusiast
</p>

<p align="center">
Turning data into insights and ideas into software.
</p>

---

## 👩‍💻 About Me

🎓 I am a **Management Information Systems graduate**.

📊 I am currently developing my skills in **Data Analytics, Data Visualization and Python**.

💻 I enjoy developing web applications and data-driven projects that solve real-world problems.

📈 I work with **data cleaning, exploratory data analysis, visualization, statistics and machine learning**.

🤖 I am also exploring **deep learning and computer vision** through practical projects.

🚀 I continuously improve my technical skills by building real-world projects and experimenting with new technologies.

🎯 My career goal is to become a **Data Analyst** while continuing to strengthen my software development skills.

---

## 🌱 Currently Learning

* 📊 Data Analytics
* 📈 Power BI
* 🐍 Python
* 🗄 SQL
* 📉 Statistics
* 🤖 Machine Learning
* 🧠 Deep Learning
* 👁️ Computer Vision
* 📊 Data Visualization
* 🎨 Interactive Dashboard Development

---

# 💻 Tech Stack

### Programming Languages

<p align="left">
<img src="https://skillicons.dev/icons?i=python,php,kotlin,dart"/>
</p>

### Web Development

<p align="left">
<img src="https://skillicons.dev/icons?i=html,css,tailwind,js"/>
</p>

### Database

<p align="left">
<img src="https://skillicons.dev/icons?i=mysql,sqlite,postgres"/>
</p>

### Tools

<p align="left">
<img src="https://skillicons.dev/icons?i=git,github,vscode"/>
</p>

### Data Analytics

* Microsoft Excel
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Plotly
* SciPy
* Scikit-learn
* XGBoost
* Data Cleaning
* Exploratory Data Analysis (EDA)
* Statistical Analysis
* Data Visualization
* Power BI

### Machine Learning & AI

* Scikit-learn
* Linear Regression
* XGBoost
* Feature Engineering
* Model Evaluation
* Cross Validation
* TensorFlow / Keras
* PyTorch
* Hugging Face Transformers
* Wav2Vec2
* ONNX
* Librosa
* MobileNetV2
* Transfer Learning
* Data Augmentation
* Grad-CAM
* PCA
* t-SNE

### Application Development

* Streamlit
* PHP
* HTML
* CSS
* JavaScript

---

# 🚀 Featured Projects

## 🎙️ VoiceSense AI — Speech Emotion Recognition

A **Wav2Vec2-based Speech Emotion Recognition (SER)** project that classifies emotions from speech audio.

The model was fine-tuned on the **RAVDESS** dataset with a **speaker-independent** setup and evaluated on actors it never saw during training.

The system predicts four emotions:

* 😐 Neutral
* 😊 Happy
* 😢 Sad
* 😠 Angry

```text
Audio Input
      ↓
Audio Preprocessing
      ↓
Wav2Vec2 Feature Extractor
      ↓
Fine-Tuned Emotion Classifier
      ↓
Emotion Probabilities
      ↓
Calibration
      ↓
Streamlit Interface
```

### Key Features

* 🎙️ Audio file upload and microphone recording
* 🧠 Wav2Vec2 fine-tuning with PyTorch
* 🧪 Speaker-independent split (Train: Actors 1–16, Validation: 17–20, Test: 21–24)
* 🎯 Class-wise logit offset calibration, optimized on the validation set only
* 📊 Emotion probabilities and confidence analysis
* ⚠️ Low-confidence warning (below 60%) that also shows the second most likely emotion
* 🔊 Real-world self test with my own voice recordings
* ⚡ PyTorch / ONNX CPU inference benchmark
* 🖥️ Interactive Streamlit interface

### Results (Unseen Test Speakers)

| Model                    |  Accuracy |  Macro-F1 |
| ------------------------ | --------: | --------: |
| Wav2Vec2 Zero-Shot       |     0.286 |     0.115 |
| Fine-Tuned Wav2Vec2      |     0.786 |     0.781 |
| Fine-Tuned + Calibration | **0.821** | **0.811** |

The test set was not used during calibration to avoid data leakage.

### Technical Notes

* **Audio windowing:** 5-second windows; longer recordings are split and the window probabilities are averaged.
* **Overfitting control:** 3 epochs, frozen feature encoder and best-checkpoint selection by validation Macro-F1.
* **ONNX benchmark:** ONNX FP32 produced the same predictions as PyTorch (20/20). INT8 quantization reduced model size by about 4x but was slower on CPU for this model, so the final version uses PyTorch + safetensors.

> ⚠️ The model is trained on acted English speech (RAVDESS) and has not yet been validated on other datasets or natural conversations. Confidence values should not be interpreted as true probabilities.

**Technologies**

Python • PyTorch • Hugging Face Transformers • Wav2Vec2 • Librosa • Scikit-learn • ONNX • Streamlit

---

## 🧠 Brain Tumor Analysis & Classification

A deep learning-based MRI image classification project developed with **TensorFlow/Keras and Streamlit**.

The project classifies MRI images into four different classes:

* Glioma
* Meningioma
* No Tumor
* Pituitary

The application combines data exploration, model evaluation, real-time prediction and model interpretability in an interactive dashboard.

### Key Features

* 📊 Exploratory Data Analysis
* 🧠 4-class MRI classification
* 🔬 MobileNetV2 Transfer Learning
* 🔄 3-Fold Stratified Cross Validation
* 📈 Confusion Matrix
* 📋 Classification Report
* 🔥 Grad-CAM visualization
* 🧬 PCA and t-SNE
* 🖥️ Interactive Streamlit Dashboard

**Model:** MobileNetV2 + Transfer Learning

**Average Test Accuracy:** 80.9% ± 1.1%

**Technologies**

Python • TensorFlow • Keras • MobileNetV2 • Streamlit • Scikit-learn • NumPy • Pandas • Matplotlib

> ⚠️ This project is developed for educational, research and portfolio purposes. It is not intended for medical diagnosis or clinical decision-making.

---

## 📊 DataInsight Platform

An interactive **data analysis and automated reporting platform** developed with Python and Streamlit.

The application allows users to upload datasets and perform automated data exploration and analysis.

### Key Features

* 📂 CSV / Excel data upload
* 🧹 Data cleaning
* 🔍 Missing value analysis
* 📊 Exploratory Data Analysis
* 📈 Statistical analysis
* 🔗 Correlation analysis
* 📉 Data visualization
* 📄 Automated PDF reporting
* 📊 Automated Excel reporting
* 🖥️ Interactive Streamlit dashboard

**Technologies**

Python • Pandas • NumPy • SciPy • Matplotlib • Seaborn • Streamlit • ReportLab • OpenPyXL

---

## 🏠 Kira Fiyatı Tahmini — İzmir / Buca

A machine learning project focused on analyzing rental housing data from **İzmir / Buca** and predicting rental prices based on property characteristics.

### Project Process

```text
Data Collection
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
Exploratory Data Analysis
      ↓
Model Training
      ↓
Cross Validation
      ↓
Model Evaluation
      ↓
Rental Price Prediction
```

### Key Topics

* Data preprocessing
* Missing value handling
* Outlier analysis
* Feature engineering
* One-Hot Encoding
* Exploratory Data Analysis
* Linear Regression
* XGBoost
* GridSearchCV
* Cross Validation
* Model evaluation

**Technologies**

Python • Pandas • NumPy • Matplotlib • Seaborn • Scikit-learn • XGBoost

---

## 💬 WhatsApp Chat Analysis

An interactive **WhatsApp conversation analysis application** developed with Python and Streamlit.

The project transforms exported WhatsApp conversations into meaningful statistics and visualizations.

### Key Features

* 👥 User activity analysis
* 📅 Daily and monthly message trends
* ⏰ Time-based analysis
* 📝 Word frequency analysis
* 🔤 Bigram analysis
* ☁️ Word Cloud
* 😊 Emoji analysis
* 📊 Activity statistics
* 📋 Raw and processed data views
* 🖥️ Interactive Streamlit interface

**Technologies**

Python • Pandas • Streamlit • Matplotlib • WordCloud • Emoji • Regex

---

## 🎧 Spotify Listening History Analysis

An interactive data analysis project that explores Spotify listening history and identifies listening habits and trends.

### Key Features

* 🎤 Most listened artists
* 🎵 Most listened songs
* 📅 Yearly listening trends
* 📆 Monthly listening trends
* 🎼 Music and genre analysis
* ⏰ Listening habits
* ⏭️ Skip behavior
* 🔄 Listening behavior over time
* 📊 Interactive visualizations

The application supports different Spotify data formats including **CSV, JSON and ZIP** files.

**Technologies**

Python • Pandas • Plotly • Streamlit

---

## 💰 AI Budget Tracking System

An AI-powered web application designed to help university students manage their budgets, monitor expenses and improve financial planning.

**Technologies**

PHP • HTML • CSS • JavaScript • MySQL

---

## 📊 Rental House Data Analysis

A data analysis project focused on cleaning, preprocessing and exploring rental housing data using Python.

### Key Topics

* Data cleaning
* Missing value analysis
* Categorical data analysis
* Exploratory Data Analysis
* Data visualization

**Technologies**

Python • Pandas • NumPy • Matplotlib

---

## 🌊 Kağıt Gemi

A web application where users can anonymously share thoughts and emotions through digital paper boats.

**Technologies**

HTML • CSS • JavaScript • PHP

---

## 🛡️ KAYRA

A social impact-oriented web platform designed to raise awareness about violence against women, preserve memories and provide access to support resources.

**Technologies**

HTML • CSS • JavaScript • PHP

---

# 📈 My Data Analytics Journey

```text
Data Collection
      ↓
Data Cleaning
      ↓
Data Transformation
      ↓
Exploratory Data Analysis
      ↓
Statistical Analysis
      ↓
Data Visualization
      ↓
Machine Learning
      ↓
Deep Learning
      ↓
Interactive Dashboards
      ↓
Automated Reporting
```

My projects allow me to practice different stages of the data lifecycle while combining **analytics, visualization, machine learning and software development**.

---

# 🧠 Areas of Interest

```text
📊 Data Analytics
      │
      ├── Data Cleaning
      ├── EDA
      ├── Statistics
      └── Data Visualization

🤖 Machine Learning
      │
      ├── Regression
      ├── Classification
      ├── Feature Engineering
      └── Model Evaluation

🧠 Deep Learning
      │
      ├── Transfer Learning
      ├── Computer Vision
      ├── CNN
      └── Model Interpretability

📈 Data Applications
      │
      ├── Streamlit
      ├── Power BI
      └── Automated Reporting

💻 Software Development
      │
      ├── Web Development
      ├── PHP
      ├── JavaScript
      └── SQL
```

---

# 📂 Project Categories

| Category            | Projects                                                                |
| ------------------- | ----------------------------------------------------------------------- |
| 📊 Data Analytics   | DataInsight, WhatsApp Analysis, Spotify Analysis, Rental House Analysis |
| 🤖 Machine Learning | Kira Price Prediction                                                   |
| 🧠 Deep Learning    | Brain Tumor Analysis, VoiceSense AI                                     |
| 💻 Web Development  | AI Budget Tracking, Kağıt Gemi, KAYRA                                   |
| 📈 Dashboard        | DataInsight, WhatsApp Analysis, Spotify Analysis, Brain Tumor Analysis, VoiceSense AI |

---

# 📫 Connect With Me

<p align="left">

📧 **Email:** [s.cansutopci@gmail.com](mailto:s.cansutopci@gmail.com)

💼 **LinkedIn:** https://linkedin.com/in/s-cansu-topci/

🌐 **GitHub:** https://github.com/c2nsu

</p>

---

<p align="center">

### ⭐ Thank you for visiting my profile!

*"Building software, exploring data and continuously learning."*

</p>

<p align="center">
<img src="https://komarev.com/ghpvc/?username=c2nsu&label=Profile%20Views&color=2563EB&style=for-the-badge"/>
</p>
