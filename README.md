# Ball Bearing Sensor Data Anomaly Detection

This project implements an **LSTM Autoencoder** to detect anomalies in ball bearing sensor data. The system analyzes time-series data from sensors to monitor wear and detect potential failures, enabling predictive maintenance.

## Overview

Rotational ball bearings are critical components in many mechanical systems. Monitoring their condition through sensor data can prevent unexpected failures and costly downtimes. This project uses machine learning to process sensor data and detect anomalies indicating wear or failure.

### Key Features:
- Signal data analysis for bearings
- Data preprocessing, including feature engineering and Fourier Transform
- LSTM autoencoder for anomaly detection
- Visualization of anomalies and reconstruction loss

---

## Features

- **Feature Engineering**:
  - Aggregates and processes raw sensor data into meaningful metrics.
  - Applies Fast Fourier Transform (FFT) to analyze frequency domain characteristics.

- **Modeling**:
  - LSTM autoencoder for reconstructing normal behavior.
  - Detection of deviations (anomalies) using reconstruction loss.

- **Visualization**:
  - Time-series plots of sensor data.
  - Reconstruction loss distributions to identify thresholds for anomaly detection.

---

## Dependencies

Ensure you have the following libraries installed:

- Python 3.7+
- Pandas
- NumPy
- scikit-learn
- TensorFlow/Keras
- Matplotlib
- Seaborn






## Data

The project uses sensor data from ball bearings. The dataset should include time-series sensor readings (e.g., vibration, noise) for multiple bearings.

- **Input**: CSV files containing raw sensor data.
- **Preprocessing**: Feature aggregation, normalization, and FFT transformation.

---

## How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Gireesh-Guntupalli/Anomaly-Detection.git
   cd Anomaly-Detection

## Results

### Reconstruction Error Threshold
The model learns normal behavior and uses reconstruction error to detect anomalies.

### Anomaly Detection
Bearings with higher reconstruction loss are flagged as potential failures.

### Visualization
Loss distribution plots and time-series anomaly detection graphs are generated to help interpret the results.

Install dependencies using:
```bash
pip install -r requirements.txt
