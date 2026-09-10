# 🩺 DermaVision AI

**AI-assisted skin lesion classification using YOLO26M-CLS and the HAM10000 dataset.**

DermaVision AI is an academic research prototype that analyzes dermoscopic skin lesion images and predicts one of **seven diagnostic classes** using a trained deep-learning model.

> ⚠️ **Research Prototype:** This application is for academic and educational purposes only. It is not a medical diagnostic device and should not replace professional medical evaluation.

---

## 🚀 Live Demo

**Streamlit App:**
https://dermavision-ai-8la8tdzsxtjvaaewstjzsj.streamlit.app/

---

## 📸 Application Screenshots

<img width="1917" height="870" alt="Screenshot 2026-09-10 202557" src="https://github.com/user-attachments/assets/fbb52fce-cc0f-49d0-bb45-7350039870d6" />

### Skin Lesion Assessment

<img width="1917" height="865" alt="Screenshot 2026-09-10 202703" src="https://github.com/user-attachments/assets/526195ec-4609-4dad-91a4-fde87c16d027" />

### Prediction Result

<img width="1917" height="867" alt="Screenshot 2026-09-10 202716" src="https://github.com/user-attachments/assets/02dce917-887a-4621-a2ae-37f607cc9bac" />
<img width="1917" height="860" alt="Screenshot 2026-09-10 202726" src="https://github.com/user-attachments/assets/21575ccc-910c-4c61-b4e2-5aaf358445ea" />

### Report Generation

<img width="1917" height="922" alt="Screenshot 2026-09-10 202806" src="https://github.com/user-attachments/assets/10e4b226-ad53-45c7-871d-26a4fcf470aa" />


## ⚙️ How It Works

1. **Open the application**
   The home page displays model information, architectures, and performance metrics.

2. **Upload an image**
   Go to **Skin Lesion Assessment** and upload a dermoscopic skin lesion image.

3. **AI Classification**
   The YOLO26M-CLS model processes the image and predicts the most likely class.

4. **View Results**
   The prediction report displays the predicted class, confidence score, probability distribution, and Top-3 predictions.

5. **View Research Results**
   Users can scroll down to see model and dataset information, including input resolution, split strategy, imbalance strategy, and evaluation metrics.

---

## 🧠 Model & Dataset

| Item                  | Details                                    |
| --------------------- | ------------------------------------------ |
| **Model**             | YOLO26M-CLS                                |
| **Dataset**           | HAM10000                                   |
| **Classes**           | 7                                          |
| **Input Resolution**  | 224 × 224                                  |
| **Training Strategy** | Lesion-aware split + moderate oversampling |
| **Best Model**        | Oversampled YOLO26M-CLS                    |

### Diagnostic Classes

* Actinic Keratoses / Bowen's Disease (`akiec`)
* Basal Cell Carcinoma (`bcc`)
* Benign Keratosis-like Lesions (`bkl`)
* Dermatofibroma (`df`)
* Melanoma (`mel`)
* Melanocytic Nevus (`nv`)
* Vascular Lesions (`vasc`)

---

## 📊 Test Performance

Results on the held-out test set:

| Metric                |      Score |
| --------------------- | ---------: |
| **Test Accuracy**     | **83.16%** |
| **Balanced Accuracy** | **68.98%** |
| **Macro F1 Score**    | **71.77%** |
| **Macro ROC AUC**     | **96.33%** |
| **Melanoma Recall**   | **49.10%** |

---

## 🛠️ Technologies

* **Python**
* **Streamlit**
* **Ultralytics YOLO**
* **PyTorch**
* **Pillow**
* **OpenCV**
* **NumPy**
* **Pandas**
* **Altair**

---

## 📁 Project Structure

```text
dermavision-ai/
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
│
└── final_model/
    └── YOLO26M_HAM10000_FINAL_best.pt
```

---

## 💻 Run Locally

```bash
git clone https://github.com/Sheetal-Patel17/dermavision-ai.git
cd dermavision-ai
python -m pip install -r requirements.txt
python -m streamlit run app.py
```

The application will open at:

```text
http://localhost:8501
```

---

## ☁️ Deployment

The application is deployed using **Streamlit Community Cloud**.

**Live App:**
https://dermavision-ai-8la8tdzsxtjvaaewstjzsj.streamlit.app/

---

## ⚠️ Disclaimer

DermaVision AI is an **academic research prototype**.

The model predictions are not medical diagnoses and should not replace examination, dermoscopy, histopathology, or advice from a qualified healthcare professional.

---

## 👩‍💻 Author

**Sheetal Patel**
B.Tech Information Technology — Marwadi University

**GitHub:** https://github.com/Sheetal-Patel17
**LinkedIn:** https://linkedin.com/in/sheetal-patel17
