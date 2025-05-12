# LSTM-BASED-PRICE-PREDICTION-AND-BUFFER-OPTIMIZATION

## Project Overview
Our Smart India Hackathon project aims at using an LSTM (Long Short-Term Memory) neural network to predict **zone-wise wholesale prices** of agricultural commodities in India to optimize the buffer stock of the commodities. It handles time series forecasting by creating lag features and training separate LSTM models for each zone. 

## Features
- **Zone-wise Price Prediction**:Uses Long Short-Term Memory (LSTM) neural networks to predict future wholesale prices for tomatoes, onions, and wheat and predictions are made on a monthly basis, tailored to each geographical zone (e.g., North, South, East, West, Central, Northeast).
- **Deep Learning Integration**: Incorporates time-series deep learning with Keras/TensorFlow and trained on historical pricing data with sliding window techniques for input sequences.
- **Smart Data Preprocessing**:Handles missing values, encoding, and scaling using MinMaxScaler and automatically converts string date fields to datetime objects and sets them as time-series indices.
- **Visualization Support**: Includes matplotlib plots to compare actual vs predicted prices and helps government stakeholders and policy makers quickly analyze pricing trends.
- **Scalable for More Commodities**:Modular pipeline can be extended to more crops with minor configuration changes.
- **Buffer Stock Forecasting (Future Enhancement)**:Designed to be extended with buffer stock modules to help predict storage requirements and prevent shortages/surpluses..
- **Evaluation Metrics**:Uses Root Mean Square Error (RMSE) for model evaluation and easy integration with metrics dashboard or Excel reports.

---

## Project Structure
```
|── Source Code/ 
|   ├── SIH/
|   |  ├── sih_pro.ipynb           
|   |  ├── sih_pro2.ipynb
|   ├── SIH DATAS/
|   |  ├── onion.ipynb
|   |  ├── wheat.ipynb
|   |  ├── preprocess_and_clean.ipynb
       
```

---

## Installation
### Prerequisites
Ensure you have the following installed:
- Python 3.7+
- Pandas
- Tensorflow
- matplotlib
- NumPy
- os


### Setup Instructions
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/LSTM-BASED-PRICE-PREDICTION-AND-BUFFER-OPTIMIZATION.git
   cd LSTM-BASED-PRICE-PREDICTION-AND-BUFFER-OPTIMIZATION
   ```
2. Install dependencies:
   ```sh
   pip install -r requirements.txt
   ```
 3.Download the pretrained `LSTM_model.h5` model:
   - Extract using:
     ```sh
     bzip2 -d LSTM_model.h5.bz2
     ```
   - Place the extracted `.h5` file inside the `models/` folder.
   
4. Run the system:
   ```sh
   python sih_pro
   python sih_pro2
   ```

---


---

## Contributors
- **Gokulakrishnan S** https://github.com/gokulispro

---

## License
This project is licensed under the MIT License.
