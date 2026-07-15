# Soil Strength Prediction using Artificial Neural Networks (ANN)

This repository contains a deep learning approach using **TensorFlow/Keras** to predict key geotechnical engineering properties of stabilized soil—specifically **California Bearing Ratio (CBR)** and **Unconfined Compressive Strength (UCS)**.

## 🚀 How it Works

The model uses an Artificial Neural Network (ANN) to map soil stabilization mix designs and physical properties to structural strength outputs.

### **Features & Workflow:**
* **Inputs (7 features):** 
  * Stabilizers: Fly Ash, Lime, Cement
  * Geotechnical limits: Liquid Limit (L.L), Plastic Limit (P.L)
  * Compaction parameters: Optimum Moisture Content (OMC), Maximum Dry Density (MDD)
* **Outputs (2 targets):** 
  * California Bearing Ratio (CBR)
  * Unconfined Compressive Strength (UCS)
* **Data Preprocessing:** Standardized using `MinMaxScaler` from `scikit-learn` to ensure stable training.
* **Model Architecture:** A feedforward neural network (`Sequential` model) with:
  * 1 Hidden Layer (10 neurons, `tanh` activation)
  * 1 Output Layer (2 neurons, `tanh` activation)
  * Trained using the `Adam` optimizer and Mean Squared Error (`mse`) loss over 200 epochs.
