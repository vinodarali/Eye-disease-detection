# 👁️ Retinal OCT Eye Disease Detection Platform

An AI-powered web application for classifying Optical Coherence Tomography (OCT) retinal images to identify common eye diseases including **Choroidal Neovascularization (CNV)**, **Diabetic Macular Edema (DME)**, **Drusen**, and **Normal Retina**.

---

## 🌟 Key Features

- **Automated OCT Classification:** Instant diagnostic support using a deep learning classifier based on **MobileNetV3**.
- **Interactive Web Interface:** Streamlit-powered dashboard for uploading OCT scans and visualizing predictions.
- **Clinical Insights & Guidance:** Detailed disease overview, recommended treatment options, and lifestyle guidance for healthcare professionals and patients.
- **GPU Accelerated & Optimized:** Efficient model loading with `@st.cache_resource` for low-latency predictions.

---

## 🦠 Detectable Retinal Conditions

| Condition | Description | Clinical Impact |
| :--- | :--- | :--- |
| **CNV** | Choroidal Neovascularization | Abnormal blood vessel growth under the retina, common in wet AMD. |
| **DME** | Diabetic Macular Edema | Fluid accumulation in the macula caused by diabetic retinopathy. |
| **DRUSEN** | Drusen Deposits | Yellowish extracellular deposits beneath the retina, early AMD indicator. |
| **NORMAL** | Normal Retina | Preserved foveal contour without pathological alterations. |

---

## 🛠️ Tech Stack & Dependencies

- **Frontend / Dashboard:** Streamlit
- **Deep Learning Framework:** TensorFlow / Keras (MobileNetV3 architecture)
- **Data & Image Processing:** NumPy, Pillow, Scikit-Learn
- **Visualization:** Matplotlib, Seaborn
- **Large File Storage:** Git LFS (for `Trained_Model.keras`)

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- Git & Git LFS installed

### Installation & Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/vinodarali/Eye-disease-Detection.git
   cd Eye-disease-Detection
   ```

2. **Pull Large Files (Model Weight):**
   ```bash
   git lfs pull
   ```

3. **Create & Activate a Virtual Environment:**
   ```bash
   python -m venv .venv
   # Windows
   .venv\Scripts\activate
   # macOS/Linux
   source .venv/bin/activate
   ```

4. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

5. **Run the Application:**
   ```bash
   streamlit run app.py
   ```

---

## 📁 Repository Structure

```
├── app.py                   # Streamlit web application
├── recommendation.py        # Medical recommendations & Markdown resources
├── requirements.txt         # Project dependencies
├── runtime.txt              # Python runtime configuration
├── Trained_Model.keras      # Trained Keras model (Git LFS tracked)
├── training_model.ipynb     # Jupyter notebook for model training
├── model_prediction.ipynb   # Jupyter notebook for inference & testing
├── .gitattributes           # Git LFS settings
├── .gitignore               # Ignored files (venv, datasets, cache)
└── README.md                # Project documentation
```

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).
