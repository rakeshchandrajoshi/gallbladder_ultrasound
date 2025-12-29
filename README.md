# Self-Attention-Guided Residual Deep Neural Network for Gallbladder Disease Diagnosis

📌 **Official implementation of the model proposed in:**

> **Self-attention-guided residual deep neural network with multi-scale dilated feature extraction for automated gallbladder disease diagnosis in ultrasound imaging**  
> *Computer Methods and Programs in Biomedicine*, Volume 271, November 2025, 109020  
> https://doi.org/10.1016/j.cmpb.2025.109020

---

## 📖 Overview

Gallbladder diseases such as gallstones, cholecystitis, adenomyomatosis, carcinoma, and perforation can lead to severe complications if not diagnosed early. Ultrasound imaging is the primary diagnostic modality, but manual interpretation is challenging due to noise, low contrast, and inter-observer variability.

This repository provides the **official source code and trained model** for a **Self-Attention-Guided Residual Deep Neural Network with Multi-Scale Dilated Feature Extraction**, designed for **fine-grained classification of nine gallbladder diseases from ultrasound images**.

The proposed model integrates:
- **Multi-scale dilated convolutions** for capturing local and global contextual features
- **Self-attention mechanisms** to focus on disease-relevant regions
- **Residual connections** to preserve spatial information and stabilize deep training

The framework achieves **state-of-the-art performance** while remaining lightweight and computationally efficient.

---

## 🚀 Key Contributions

- ✔️ Novel **attention-aware residual CNN** for multi-class gallbladder disease classification  
- ✔️ **Nine-class classification** using heterogeneous ultrasound data  
- ✔️ Robust to **noise, artifacts, and intra-class variability**  
- ✔️ **High accuracy (99.17%)** with real-time inference capability  
- ✔️ Explainable predictions using **Grad-CAM visualizations**  
- ✔️ Lightweight model suitable for **clinical and point-of-care deployment**

---

## 🩺 Gallbladder Disease Classes

The model classifies the following **nine disease categories**:

1. Gallstones  
2. Cholecystitis  
3. Membranous and Gangrenous Cholecystitis  
4. Perforation  
5. Polyps and Cholesterol Crystals  
6. Adenomyomatosis  
7. Carcinoma  
8. Abdomen and Retroperitoneal Pathology  
9. Various Causes of Gallbladder Wall Thickening  

---

## 📊 Performance Highlights

| Metric | Value |
|------|------|
| **Accuracy** | **99.17%** |
| Precision | 99.17% |
| Recall | 98.94% |
| AUC | 1.00 |
| Model Size | 14.33 MB |
| Parameters | 3.76M |
| Inference Speed | ~120 images/sec |

The model outperforms DenseNet-201, MobileNet, Inception-v3, and VGG-19 in both **accuracy and efficiency**.

---

## 🗂 Repository Contents
📁 gallbladder_ultrasound
│
├── gallbladder_ultrasound_self_attention.ipynb
│ └── Jupyter Notebook containing:
│ • Data preprocessing
│ • Model architecture
│ • Training and validation
│ • Evaluation metrics
│ • Grad-CAM explainability
│
├── model-031-0.979685-0.992509.keras
│ └── Pre-trained Keras model
│ • Ready for inference
│ • Best-performing checkpoint
│
└── README.md




---

## 📦 Dataset

The model is trained and evaluated on a **large-scale, publicly available dataset**:

**Gallbladder Diseases Dataset**  
- **10,692 ultrasound images**
- Collected over 4 years
- Multiple hospitals and ultrasound machines
- Expert radiologist annotations

📎 **Dataset Link:**  
Turki et al., *Gallbladder Diseases Dataset*, Mendeley Data (2024)  
DOI: 10.17632/r6h24d2d3y.1

---

## ⚙️ Requirements

- Python ≥ 3.8  
- TensorFlow / Keras  
- NumPy  
- OpenCV  
- Matplotlib  
- Scikit-learn  

Recommended GPU for training (tested on NVIDIA DGX A100).

---

## ▶️ Usage

### 1️⃣ Clone the repository
```bash
git clone https://github.com/rakeshchandrajoshi/gallbladder_ultrasound.git
cd gallbladder_ultrasound




````

### 2️⃣ Run the notebook

Open and execute:

```bash
gallbladder_ultrasound_self_attention.ipynb
```

### 3️⃣ Load the pre-trained model (example)

```python
from tensorflow.keras.models import load_model

model = load_model("model-031-0.979685-0.992509.keras")
```

---

## 🔍 Explainability (Grad-CAM)

The model includes **Grad-CAM–based visual explanations** highlighting clinically relevant regions such as:

* Gallstones and acoustic shadows
* Thickened gallbladder walls
* Irregular carcinoma lesions
* Perforation boundaries

These visualizations improve **clinical trust and interpretability**.

---

## 📌 Citation

If you use this code or model, **please cite the following paper**:

```bibtex
@article{Rashid2025GallbladderAI,
  title={Self-attention-guided residual deep neural network with multi-scale dilated feature extraction for automated gallbladder disease diagnosis in ultrasound imaging},
  journal={Computer Methods and Programs in Biomedicine},
  volume={271},
  pages={109020},
  year={2025},
  doi={10.1016/j.cmpb.2025.109020},
  author={Rashid, Suzain and Das, Chandan J. and Chauhan, Anshika and Aggarwal, Garima and Joshi, Rakesh Chandra and Burget, Radim and Dutta, Malay Kishore}
}
```

---

## ⚠️ Disclaimer

This repository is intended **for research and academic use only**.
The model is **not a substitute for professional medical diagnosis** and should not be used as a standalone clinical decision-making tool without proper validation and regulatory approval.

---

## 📬 Contact

For questions or collaborations:

* **Corresponding Author:**
  **Dr. Malay Kishore Dutta**
  📧 [malaykishoredutta@gmail.com](mailto:malaykishoredutta@gmail.com)

* **Code Maintainer:**
  **Dr. Rakesh Chandra Joshi**
  📧 [rakeshchandraindia@gmail.com](mailto:rakeshchandraindia@gmail.com)

---

⭐ If you find this work useful, please consider **starring the repository** and **citing the paper**.

```

---

If you want, I can also:
- Add **badges** (DOI, journal, TensorFlow, license)
- Write a **short GitHub description tagline**
- Optimize it for **Google Scholar / GitHub SEO**
- Add a **demo inference snippet** with sample input/output

Just tell me 👍
```
