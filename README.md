# Admission Prediction using Artificial Neural Network (ANN)

This project uses a deep learning model to predict the chances of graduate school admission based on various academic and research parameters.

---

## 📋 Overview

This Jupyter notebook implements a neural network regression model to predict admission probability using the Graduate Admission dataset. The model considers factors such as GRE scores, TOEFL scores, university rating, and other academic metrics.

---

## 📊 Dataset

The dataset includes the following features:

* **GRE Score:** (out of 340)
* **TOEFL Score:** (out of 120)
* **University Rating:** (1–5)
* **SOP:** Statement of Purpose strength (1–5)
* **LOR:** Letter of Recommendation strength (1–5)
* **CGPA:** (out of 10)
* **Research:** Research experience (0 or 1)
* **Chance of Admit:** Target variable (0 to 1)

---

## 🧠 Model Architecture

The neural network consists of:

* **Input Layer:** 7 features
* **Hidden Layer 1:** 7 neurons with ReLU activation
* **Hidden Layer 2:** 7 neurons with ReLU activation
* **Output Layer:** 1 neuron with linear activation (regression)

---

## 🛠️ Dependencies

Ensure you have Python 3.x installed along with the following libraries:

* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* TensorFlow / Keras

---

## 📈 Performance

* **R² Score:** ~0.79 on the test set

---

## 🚀 How to Run

1. **Install required dependencies:**

   ```bash
   pip install pandas numpy matplotlib scikit-learn tensorflow keras
   

2. **Open the Jupyter notebook:**
```bash
jupyter notebook admission_prediction.ipynb

```


3. **Run all cells sequentially.**

---

## 📝 Key Steps

1. **Data Loading:** Load the `Admission_Predict.csv` dataset.
2. **Data Preprocessing:**
* Remove the `Serial No.` column.
* Split into features ($X$) and target ($y$).
* Scale features using `MinMaxScaler`.


3. **Model Building:** Create a Sequential neural network with 3 layers.
4. **Model Training:** Train for 100 epochs with a validation split.
5. **Evaluation:** Calculate R² score and visualize training loss.

---

## 📊 Results Visualization

The notebook includes a plot showing training and validation loss over epochs to monitor model performance and convergence.

---

## 📁 File Structure

```text
.
├── admission_prediction.ipynb   # Main notebook
└── README.md                    # Project documentation

```

---

## 🔄 Future Improvements

* Hyperparameter tuning (learning rate, batch size, optimizer)
* Experimenting with different network architectures
* Feature engineering
* Applying K-Fold Cross-Validation

---

## 📚 References

* **Dataset:** Graduate Admission dataset from Kaggle
* **Framework:** TensorFlow / Keras
