<p align="center">
    <img src="https://img.icons8.com/?size=512&id=55494&format=png" align="center" width="30%">
</p>
<h1 align="center">THALASSEMIA-PREDICTION-SYSTEM</h1>
<p align="center">
	<em><code>AI-powered blood smear image analysis for rapid Thalassemia detection</code></em>
</p>
<p align="center">
	<img src="https://img.shields.io/github/license/shlokkku/thalassemia-prediction-system?style=default&logo=opensourceinitiative&logoColor=white&color=982123" alt="license">
	<img src="https://img.shields.io/github/last-commit/shlokkku/thalassemia-prediction-system?style=default&logo=git&logoColor=white&color=982123" alt="last-commit">
	<img src="https://img.shields.io/github/languages/top/shlokkku/thalassemia-prediction-system?style=default&color=982123" alt="repo-top-language">
	<img src="https://img.shields.io/github/languages/count/shlokkku/thalassemia-prediction-system?style=default&color=982123" alt="repo-language-count">
</p>
<br>

## 🔗 Table of Contents

- [📍 Overview](#-overview)
- [👾 Features](#-features)
- [📁 Project Structure](#-project-structure)
  - [📂 Project Index](#-project-index)
- [🚀 Getting Started](#-getting-started)
  - [☑️ Prerequisites](#-prerequisites)
  - [⚙️ Installation](#-installation)
  - [🤖 Usage](#🤖-usage)
  - [🧪 Testing](#-🧪-testing)
- [📌 Project Roadmap](#-project-roadmap)
- [🔰 Contributing](#-contributing)
- [🎗 License](#-license)
- [🙌 Acknowledgments](#-acknowledgments)

---

## 📍 Overview

Thalassemia Prediction System is a machine learning-powered application for detecting signs of Thalassemia from blood smear images.  
It leverages deep learning models, packaged in an interactive web app (Streamlit), to assist clinicians and researchers in rapid, automated screening for Thalassemia trait or disease.

- **Core ML Notebook:** Contains all data preparation, model training, evaluation, and export logic (see `thalassemia_prediction.ipynb`).
- **Web App:** User-friendly UI for uploading images and getting instant predictions (see `app.py`).

---

## 👾 Features

- **Automated Detection:** Upload a blood smear image (JPG/PNG), get instant prediction: "Thalassemia" or "Normal".
- **Deep Learning Model:** Uses a pre-trained TensorFlow/Keras model for image classification.
- **Confidence Score:** Displays prediction confidence for transparency.
- **Secure Model Handling:** Model weights are downloaded from Google Drive and loaded on demand.
- **User Interface:** Built with Streamlit for easy, interactive usage.
- **Image Preprocessing:** Robust preprocessing pipeline (resize, normalization, RGB conversion) for reliable predictions.

---

## 📁 Project Structure

```sh
└── thalassemia-prediction-system/
    ├── README.md
    ├── app.py
    ├── requirements.txt
    └── thalassemia_prediction.ipynb
```

### 📂 Project Index
<details open>
	<summary><b><code>THALASSEMIA-PREDICTION-SYSTEM/</code></b></summary>
	<details>
		<summary><b>__root__</b></summary>
		<blockquote>
			<table>
			<tr>
				<td><b><a href='https://github.com/shlokkku/thalassemia-prediction-system/blob/master/thalassemia_prediction.ipynb'>thalassemia_prediction.ipynb</a></b></td>
				<td>Jupyter Notebook for data loading, preprocessing, EDA, model training, evaluation, and export. Modular, step-by-step, fully documented ML pipeline.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shlokkku/thalassemia-prediction-system/blob/master/app.py'>app.py</a></b></td>
				<td>Streamlit-based web UI; loads model, accepts user images, preprocesses input, predicts, and displays results with confidence.</td>
			</tr>
			<tr>
				<td><b><a href='https://github.com/shlokkku/thalassemia-prediction-system/blob/master/requirements.txt'>requirements.txt</a></b></td>
				<td>Lists all dependencies: Streamlit (UI), TensorFlow (ML), Pillow (image ops), gdown (model download), numpy (numeric ops), etc.</td>
			</tr>
			</table>
		</blockquote>
	</details>
</details>

---

## 🚀 Getting Started

### ☑️ Prerequisites

- **Python** (>=3.7 recommended)
- **pip** (>=21)
- **Jupyter Notebook** (for model dev)
- **Internet connection** (to download model weights)
- **(Optional)** Streamlit CLI for running the web app

### ⚙️ Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/shlokkku/thalassemia-prediction-system
   cd thalassemia-prediction-system
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
   *Dependencies explained:*
   - **streamlit**: for web UI
   - **tensorflow**: for loading and running the model
   - **Pillow**: for image processing
   - **gdown**: for downloading model files from Google Drive
   - **numpy**: for numerical operations

---

### 🤖 Usage

**Run the Streamlit web app:**
```sh
streamlit run app.py
```
- Open the provided local URL in your browser.
- Upload a blood smear image (JPG/PNG).
- View prediction result and confidence score.

**Run/modify Jupyter notebook for model development:**
```sh
jupyter notebook thalassemia_prediction.ipynb
```
- Go through data science workflow, retrain or experiment with model.

---

### 🧪 Testing

*Manual Testing:*
- Use Streamlit UI to test with sample images.
- Validate predictions with known positive/negative samples.

*Unit Testing:*
- For advanced users, add Python `unittest` or `pytest` scripts to validate model loading, preprocessing, and inference pipeline.

---

## 📌 Project Roadmap

- [X] Deep learning model for image classification
- [X] Interactive web app for predictions
- [X] Automated model download and loading
- [ ] Add support for batch/image set predictions
- [ ] Improve model accuracy (tuning, more training data)
- [ ] Add patient data form and result logging
- [ ] Export results to PDF/CSV for clinical use

---

## 🔰 Contributing

- 💬 [Join the Discussions](https://github.com/shlokkku/thalassemia-prediction-system/discussions): Share your insights, provide feedback, or ask questions.
- 🐛 [Report Issues](https://github.com/shlokkku/thalassemia-prediction-system/issues): Submit bugs or feature requests.
- 💡 [Submit Pull Requests](https://github.com/shlokkku/thalassemia-prediction-system/blob/main/CONTRIBUTING.md): Review open PRs, and submit your own!

<details>
<summary>Contributing Guidelines</summary>

1. **Fork the Repository**
2. **Clone Locally**
   ```sh
   git clone https://github.com/shlokkku/thalassemia-prediction-system
   ```
3. **Create a New Branch**
   ```sh
   git checkout -b feature/my-feature
   ```
4. **Make Your Changes**
5. **Commit Your Changes**
   ```sh
   git commit -m 'Describe your changes'
   ```
6. **Push to github**
   ```sh
   git push origin feature/my-feature
   ```
7. **Submit a Pull Request**
</details>

<details>
<summary>Contributor Graph</summary>
<br>
<p align="left">
   <a href="https://github.com/shlokkku/thalassemia-prediction-system/graphs/contributors">
      <img src="https://contrib.rocks/image?repo=shlokkku/thalassemia-prediction-system">
   </a>
</p>
</details>

---

## 🎗 License

This project is licensed under the [MIT License](https://github.com/shlokkku/thalassemia-prediction-system/blob/main/LICENSE).

---

## 🙌 Acknowledgments

- Based on open-source ML research and clinical datasets.
- Thanks to contributors and medical advisors.
- Inspired by advancements in AI for healthcare.
