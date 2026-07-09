# 🤖 Machine Learning & Deep Learning Notebooks

> A collection of **Jupyter notebooks** covering core concepts in **Machine Learning**, **Deep Learning**, **Neural Networks**, **Intrusion Detection**, and **Signal Processing** — implemented with TensorFlow/Keras and scikit-learn.

---

## 📁 Project Structure

```
ML-DL-Notebooks/
│
├── 📊 Linear Regression/
│   ├── linear_regression_random_data.ipynb          # Linear regression on randomly generated data
│   ├── linear_regression_make_regression.ipynb      # Linear regression with sklearn make_regression
│   └── linear_regression_diabetes.ipynb             # Linear regression on the Diabetes dataset (sklearn)
│
├── 🧠 Neural Networks — Fundamentals/
│   ├── neural_network_mnist_handwritten_digits.ipynb # MLP on MNIST handwritten digits (SGD + sigmoid)
│   ├── knn_handwritten_digits_sklearn.ipynb          # KNN classifier on sklearn digits dataset
│   └── confusion_matrix_iris.ipynb                   # Confusion matrix & report on Iris (Decision Tree)
│
├── 👗 Image Classification/
│   ├── fashion_mnist_dense_network.ipynb             # Dense NN on Fashion-MNIST clothing dataset
│   ├── fashion_mnist_cnn_advanced.ipynb              # CNN with regularization on Fashion-MNIST
│   └── cnn_mnist_lenet_numbers.ipynb                 # LeNet-style CNN on MNIST digit recognition
│
├── 📈 Regression — Real Datasets/
│   ├── boston_housing_regression_mlp.ipynb           # MLP regression on Boston Housing dataset
│   ├── boston_housing_regression_project.ipynb       # Full project: Boston Housing price prediction
│   └── apple_stock_price_prediction_lstm.ipynb       # Apple (AAPL) stock price prediction with LSTM
│
├── 🔒 Cybersecurity & IDS/
│   ├── ids_nsl_kdd_ml_dl_hybrid.ipynb                # IDS on NSL-KDD: ML vs DL vs Hybrid + SMOTE
│   ├── logistic_regression_smote_ids.ipynb           # Logistic Regression with/without SMOTE (TP4)
│   └── ids_nsl_kdd_full_pipeline.ipynb               # Full IDS pipeline on NSL-KDD dataset
│
├── 🌐 Sequence & Time Series/
│   ├── rnn_lstm_internet_traffic.ipynb               # RNN/LSTM for Internet traffic prediction
│   └── diabetes_prediction_from_food.ipynb           # Diabetes rate prediction from nutritional data
│
├── 🔊 Signal Processing/
│   └── audio_denoising_cnn_autoencoder.ipynb         # Audio signal denoising with Conv1D Autoencoder
│
└── 🚀 Fine-Tuning & Advanced/
    └── llm_fine_tuning_unsloth.ipynb                 # LLM fine-tuning with Unsloth, PEFT & LoRA
```

---

## 📋 Notebooks Description

### 📊 Linear Regression

| File                                      | Description                                                                                                                                                  |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `linear_regression_random_data.ipynb`     | Implements simple linear regression on a randomly generated dataset using `sklearn.LinearRegression`. Visualizes the regression line vs. actual data points. |
| `linear_regression_make_regression.ipynb` | Uses `sklearn.make_regression` to generate a synthetic dataset and fits a linear regression model. Explores data shape and scatter plots.                    |
| `linear_regression_diabetes.ipynb`        | Applies linear regression to the sklearn Diabetes dataset. Uses a single feature, splits data into train/test, and evaluates with MSE and R² score.          |

### 🧠 Neural Networks — Fundamentals

| File                                            | Description                                                                                                                                                                |
| ----------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `neural_network_mnist_handwritten_digits.ipynb` | Builds a 3-layer MLP (sigmoid activations, SGD optimizer) on MNIST. Flattens 28×28 images to 784-dim vectors. Demonstrates one-hot encoding and categorical cross-entropy. |
| `knn_handwritten_digits_sklearn.ipynb`          | Loads the sklearn `digits` dataset and trains a K-Nearest Neighbors (k=3) classifier. Evaluates with a full classification report.                                         |
| `confusion_matrix_iris.ipynb`                   | Trains a Decision Tree on the Iris dataset and visualizes the confusion matrix with Seaborn heatmap. Includes `classification_report` for precision/recall/F1.             |

### 👗 Image Classification

| File                                | Description                                                                                                                            |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| `fashion_mnist_dense_network.ipynb` | Trains a Dense Sequential neural network on Fashion-MNIST (10 clothing categories). Uses Adam optimizer and categorical cross-entropy. |
| `fashion_mnist_cnn_advanced.ipynb`  | Implements a CNN with Conv2D, MaxPooling, Dropout, and L2 regularization on Fashion-MNIST. Includes OpenCV for image preprocessing.    |
| `cnn_mnist_lenet_numbers.ipynb`     | Implements a LeNet-style CNN (Conv2D → MaxPool → Conv2D → MaxPool → Dense) on MNIST. Achieves high accuracy on digit recognition.      |

### 📈 Regression — Real Datasets

| File                                      | Description                                                                                                                                      |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| `boston_housing_regression_mlp.ipynb`     | MLP regressor (2×64 Dense layers + ReLU) on the Boston Housing dataset. Applies z-score normalization and evaluates with MAE/MSE.                |
| `boston_housing_regression_project.ipynb` | Extended Boston Housing project with deeper analysis, normalization pipeline, and learning curve visualization.                                  |
| `apple_stock_price_prediction_lstm.ipynb` | Downloads Apple (AAPL) stock data with `yfinance`, applies MinMaxScaler, creates time sequences, and predicts closing prices with an LSTM model. |

### 🔒 Cybersecurity & IDS

| File                                  | Description                                                                                                                                                                               |
| ------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `ids_nsl_kdd_ml_dl_hybrid.ipynb`      | Complete IDS comparison on the NSL-KDD dataset: trains multiple ML models (Random Forest, SVM, etc.) vs. a Deep Learning model vs. a Hybrid approach. Handles class imbalance with SMOTE. |
| `logistic_regression_smote_ids.ipynb` | Focuses on Logistic Regression with and without SMOTE oversampling. Compares performance metrics (accuracy, F1, AUC-ROC) for imbalanced intrusion detection data.                         |
| `ids_nsl_kdd_full_pipeline.ipynb`     | Full end-to-end IDS pipeline: data download, preprocessing (OneHotEncoder, StandardScaler), model training, confusion matrix, ROC curve, and cross-validation.                            |

### 🌐 Sequence & Time Series

| File                                  | Description                                                                                                                                                                     |
| ------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `rnn_lstm_internet_traffic.ipynb`     | Generates 1000 hours of simulated internet traffic, trains an LSTM model to predict the number of connections, and evaluates with MSE and MAE.                                  |
| `diabetes_prediction_from_food.ipynb` | Simulates 500 meals with nutritional features (carbs, proteins, fats, glycemic index) and trains a Dense NN to predict the diabetes rate. Visualizes correlations with Seaborn. |

### 🔊 Signal Processing

| File                                    | Description                                                                                                                                               |
| --------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `audio_denoising_cnn_autoencoder.ipynb` | Loads a real audio signal with `librosa`, adds white Gaussian noise, and trains a Conv1D Autoencoder (encoder + decoder) to reconstruct the clean signal. |

### 🚀 Fine-Tuning & Advanced

| File                            | Description                                                                                                                                                                                                    |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `llm_fine_tuning_unsloth.ipynb` | Fine-tunes a Large Language Model using **Unsloth**, **PEFT (LoRA)**, **TRL**, and **BitsAndBytes** for 4-bit quantization. Loads a custom JSON dataset for supervised fine-tuning (SFT). Requires GPU (CUDA). |

---

## 🛠️ Tools & Technologies

| Category          | Tool / Technology                       | Role                                                |
| ----------------- | --------------------------------------- | --------------------------------------------------- |
| Language          | **Python 3**                            | All notebooks                                       |
| Deep Learning     | **TensorFlow / Keras**                  | Neural networks, CNNs, LSTMs, Autoencoders          |
| Machine Learning  | **scikit-learn**                        | Linear Regression, KNN, Decision Tree, SVM, metrics |
| Data Manipulation | **NumPy / Pandas**                      | Arrays, DataFrames, preprocessing                   |
| Visualization     | **Matplotlib / Seaborn**                | Plots, confusion matrices, learning curves          |
| Audio Processing  | **librosa**                             | Audio loading, signal analysis                      |
| Image Processing  | **OpenCV (cv2)**                        | Image preprocessing for CNN                         |
| Stock Data        | **yfinance**                            | Apple stock price download                          |
| Class Imbalance   | **imbalanced-learn (SMOTE)**            | Oversampling for IDS datasets                       |
| LLM Fine-Tuning   | **Unsloth / PEFT / TRL / BitsAndBytes** | Efficient LoRA fine-tuning with 4-bit quantization  |
| Environment       | **Google Colab / Jupyter Notebook**     | Notebook execution environment                      |
| Dataset — IDS     | **NSL-KDD**                             | Network intrusion detection benchmark dataset       |
| Dataset — Vision  | **MNIST / Fashion-MNIST**               | Handwritten digits / clothing classification        |
| Dataset — Housing | **Boston Housing**                      | Regression on real estate prices                    |

---

## 📌 Key Concepts Covered

- **Supervised Learning** — Linear Regression, KNN, Decision Trees, Logistic Regression
- **Deep Learning** — Multilayer Perceptrons (MLP), Convolutional Neural Networks (CNN), Recurrent Neural Networks (RNN/LSTM)
- **Model Evaluation** — Confusion Matrix, Classification Report, ROC-AUC, MSE, MAE, R² Score
- **Data Preprocessing** — Normalization (z-score, MinMax), One-Hot Encoding, Train/Test Split
- **Regularization** — Dropout, L2 regularization, Batch Normalization
- **Class Imbalance Handling** — SMOTE oversampling
- **Time Series Forecasting** — Sequence creation, LSTM for temporal prediction
- **Signal Processing** — Noise addition, Conv1D Autoencoder for audio denoising
- **Image Classification** — LeNet-style CNN, Fashion-MNIST with regularization
- **Intrusion Detection (IDS)** — NSL-KDD dataset, ML vs DL vs Hybrid comparison
- **LLM Fine-Tuning** — LoRA, PEFT, 4-bit quantization with Unsloth on custom datasets
- **Stock Price Prediction** — LSTM on real financial time series (Apple AAPL)

---

## ⚙️ Installation

```bash
git clone https://github.com/Yasser-02G/ML-DL-Notebooks.git
cd ML-DL-Notebooks

pip install tensorflow scikit-learn numpy pandas matplotlib seaborn \
            librosa opencv-python yfinance imbalanced-learn jupyter
```

For the LLM fine-tuning notebook (requires GPU):

```bash
pip install unsloth trl peft accelerate bitsandbytes
```

---

## 🚀 Running the Notebooks

### Locally with Jupyter:

```bash
jupyter notebook
```

### On Google Colab:

Upload any `.ipynb` file directly to [colab.research.google.com](https://colab.research.google.com) — all notebooks were originally developed on Colab.

---

## 👤 Author

**Yasser** — Network & Security Engineer

🔗 [GitHub](https://www.google.com/search?q=https%3A%2F%2Fgithub.com%2FYasser-02G)

Feel free to open an _issue_ or a _pull request_ if you have suggestions to improve this project.

---

## 📄 License

Distributed under the MIT License.
