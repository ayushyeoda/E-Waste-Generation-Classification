
# 🧠 E-Waste Image Classification using EfficientNetV2B0

This project performs image classification on electronic waste (e-waste) images using **transfer learning** with the **EfficientNetV2B0** architecture in TensorFlow and Keras.

The model is trained to classify images into **10 categories** of electronic waste like Mobile Phones, Keyboards, Printers, etc.

---

## 🚀 Features

- 📦 Dataset loading with `image_dataset_from_directory`
- 🎨 Real-time data augmentation
- 🧠 Transfer learning with EfficientNetV2B0 (pretrained on ImageNet)
- 🔁 Fine-tuning with EarlyStopping
- 📊 Evaluation: Accuracy, Confusion Matrix, Classification Report
- 🌐 Gradio interface for interactive image classification

---

## 🗂️ Dataset

The dataset is available on Kaggle:  
🔗 [E-Waste Image Dataset (Kaggle)](https://www.kaggle.com/datasets/akshat103/e-waste-image-dataset)

**Folder structure:**
```
e-waste-image-dataset/
├── Train/
├── Validation/
└── Test/
```

Each subfolder contains images for one of the 10 e-waste categories.

---

## 🧪 Model Architecture

- Base model: `EfficientNetV2B0` (without top layer)
- GlobalAveragePooling2D
- Dropout (0.2)
- Dense layer with softmax activation (10 classes)

---

## 🧰 Requirements

Install dependencies in a virtual environment:

```bash
pip install -r requirements.txt
```

**OR manually install:**
```bash
pip install tensorflow gradio matplotlib scikit-learn
```

---

## ▶️ How to Run

1. Clone the repo or upload the files to your GitHub
2. Launch the notebook:

```bash
jupyter notebook E-Waste_Classification_Cleaned.ipynb
```

3. Update the dataset path in the notebook:
```python
base_dir = './e-waste-image-dataset'
```

4. Run all cells step by step.

---

## 🖼️ Gradio Web App

The last section launches a simple Gradio web interface:

```python
iface.launch()
```

Upload any e-waste image and see the model prediction with confidence scores.

---

## 📈 Sample Output

```
Test Accuracy: 0.95
Test Loss: 0.12
```

---

## 🛠️ Author

**Ayush Agrawal**  
📍 B.Tech Computer Engineering Student  
📫 [Your Email or LinkedIn]

---

## 📄 License

This project is licensed under the MIT License.
