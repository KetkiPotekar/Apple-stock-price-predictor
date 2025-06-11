# 📈 Apple Stock Price Prediction Using Deep Learning (SimpleRNN & LSTM)

🧠 Project Overview <br/>
This project builds a deep learning model to predict Apple Inc.’s (AAPL) adjusted closing stock prices using Recurrent Neural Networks (RNNs) and Long Short-Term Memory (LSTM) networks. The model predicts stock behavior for 1-day, 5-day, and 10-day horizons using historical stock data. <br/>

The project explores sequential modeling, time-series forecasting, hyperparameter tuning, and model deployment using industry best practices. <br/>

📄 Problem Statement <br/>
Predict the adjusted closing price of Apple stock using a deep learning-based time-series approach. <br/>
Compare the performance of SimpleRNN and LSTM architectures, and evaluate their ability to forecast near-term stock behavior. <br/>

💼 Business Use Cases <br/>
📊 Stock Trading & Investment<br/>
Automated Trading: Use predicted prices for algorithmic buy/sell decisions.<br/>
Portfolio Optimization: Adjust allocations based on forecasted trends and risks.<br/>

📉 Financial Forecasting<br/>
Long-Term Investment Planning: Inform ETF, mutual fund, or retirement investment strategies.<br/>
Macroeconomic Insights: Compare with inflation, interest rates, or economic trends.<br/>

🏢 Business Intelligence <br/>
Revenue Forecasting: Apple can forecast earnings and plan investor communication.<br/>
Competitor Benchmarking: Apply model to stocks like NIO, Lucid, or Rivian for comparative analysis.<br/>

🧪 Deep Learning Research <br/>
Model Benchmarking: Extend to GRUs, Transformers, or ARIMA for comparison. <br/>
Alt-Data Integration: Enhance prediction with news sentiment, Twitter trends, or economic indicators. <br/>

🔍 Project Approach <br/>
1️⃣ Problem Understanding <br/>
Focus on predicting adjusted closing price. <br/>
Build and compare SimpleRNN and LSTM models. <br/>
Use Apple’s historical stock dataset (AAPL.csv). <br/>

2️⃣ Data Preprocessing <br/>
Load & Explore: Read CSV using pandas, examine columns and trends. <br/>
Feature Selection: Use only the Adj Close price for prediction. <br/>
Date Parsing: Convert Date to datetime and set as index.<br/>
Normalization: Scale values to [0, 1] using MinMaxScaler. <br/>
Windowing: Create sequences for time-step prediction (lookback window). <br/>

3️⃣ Model Development<br/>
a. Architecture<br/>
SimpleRNN & LSTM models using tensorflow.keras.Sequential.<br/>

b. Compilation<br/>
Loss: mean_squared_error<br/>
Optimizer: Adam (tunable with learning rate)<br/>

c. Hyperparameter Tuning <br/>
Use GridSearchCV (with Keras wrapper) to tune:<br/>
Number of units<br/>
Dropout rate<br/>
Learning rate<br/>
Batch size and epochs<br/>

d. Training<br/>
Apply EarlyStopping and ModelCheckpoint.<br/>
Split dataset into training, validation, and test sets.<br/>

4️⃣ Evaluation & Visualization <br/>
Plot predicted vs actual prices for each forecast horizon. <br/>
Use evaluation metric: Mean Squared Error (MSE). <br/>
Compare RNN vs LSTM performance visually and numerically. <br/>

5️⃣ Insights & Limitations
Discuss effectiveness in short-term and long-term trend prediction.<br/>

Limitations:<br/>
Highly sensitive to recent trends.<br/>
No external events or news data included.<br/>

📊 Results <br/>
Developed both SimpleRNN and LSTM models for: <br/>
1-day forecast<br/>

5-day forecast<br/>

10-day forecast<br/>

Achieved meaningful prediction accuracy, especially with LSTM.<br/>

Visualized trend lines to show deviation between true and predicted values.<br/>

Demonstrated effectiveness of RNN-based forecasting for sequential stock data.<br/>
