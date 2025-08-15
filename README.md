# 🚦 Traffic Sign Classification using PyTorch

This project implements a **Traffic Sign Classification** system using a custom **Convolutional Neural Network (CNN)** built with **PyTorch**.  
The dataset is sourced from [Kaggle - Traffic Signs Preprocessed](https://www.kaggle.com/), containing images of 43 different traffic sign classes.

---

## 📂 Project Structure


---

## 📊 Dataset

The dataset contains preprocessed `.pickle` files:
- **train.pickle** — Training data
- **test.pickle** — Testing data  

Each pickle file contains:
- `features` → Image data (numpy arrays)
- `labels` → Class labels (integers)

---

## ⚙️ Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/traffic-sign-classification.git
cd traffic-sign-classification

**Download and place the dataset in:**
/kaggle/input/traffic-signs-preprocessed/


Run the training script:

python traffic_sign_classification.py

🧠 Model Architecture

The TrafficNet CNN consists of:

Conv2D Layer 1: 3 → 32 filters, kernel size 3, ReLU activation

MaxPooling: 2×2

Conv2D Layer 2: 32 → 64 filters, kernel size 3, ReLU activation

MaxPooling: 2×2

Fully Connected 1: Flatten → 128 neurons, ReLU activation

Fully Connected 2: Output layer (43 classes)

🔄 Training Process

Optimizer: Adam (learning rate = 0.001)

Loss Function: CrossEntropyLoss

Epochs: 15

Batch Size: 64

Device: GPU if available, else CPU

📈 Results

The model trains for 15 epochs with both training and validation loss plotted for performance monitoring.

📌 Key Features

Custom PyTorch Dataset class for handling pickle files

Custom CNN architecture for traffic sign classification

Training/Validation split with DataLoader

Loss monitoring and visualization

📜 License

This project is licensed under the MIT License.

🙌 Acknowledgements

Dataset: Kaggle - Traffic Signs Preprocessed

PyTorch: https://pytorch.org/

