# 🧠 Anna-Coder: Autonomous Neural Network Code Generator

**Anna-Coder** is an autonomous AI agent that automatically generates and trains neural network code.
This project includes a **CNN-based binary classifier** designed to classify data across **two labels** from **16 uploaded files**.

---

## 🚀 Features

* Automated neural network code generation
* CNN binary classifier for two categories
* Easy-to-use data loading and preprocessing
* Configurable model parameters and training options
* Evaluation and inference scripts for quick testing

---

## 🗂️ Project Structure

```
anna_coder/
│
├── data/
│   ├── class_0/        # Files for label 0
│   └── class_1/        # Files for label 1
│
├── src/
│   ├── model.py        # CNN architecture
│   ├── dataset.py      # Data loading and preprocessing
│   ├── train.py        # Training script
│   ├── eval.py         # Evaluation script
│   └── utils.py        # Helper functions
│
├── configs/
│   └── default.yaml    # Model and training configuration
│
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

```bash
python -m venv .venv
source .venv/bin/activate   # or .venv\Scripts\activate on Windows
pip install -r requirements.txt
```

---

## 🧩 How to Run

### 1. Train the Model

```bash
python -m src.train --config configs/default.yaml
```

### 2. Evaluate the Model

```bash
python -m src.eval --weights outputs/best_model.pt --data_dir data
```

### 3. Run Inference

```bash
python -m src.infer --image path/to/image.jpg
```

---

## 👥 Collaborators

* **Manush Murali**
* **Sovit Nayak**
