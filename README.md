# 👋 Hi, I'm Anshul Mittal

### Computer Science Student | Data Analytics | Machine Learning | Time Series Forecasting

I'm a B.Tech Computer Science student who likes turning messy real-world data into forecasts people can actually act on.

Most of my work follows the same path: **raw data → cleaning → EDA → honest baselines → models → evaluation → explanation**. I care a lot about *fair testing*: walk-forward evaluation, no data leakage, and always checking whether a fancy model really beats the simple rule it is meant to replace.

Currently sharpening **Data Structures & Algorithms in C++**, time series modelling, and explainable ML.

---

## 🚀 What I Work On

- 📊 **Data Analytics**: EDA, cleaning, finding the patterns and outliers in real datasets
- 📈 **Time Series Forecasting**: ARIMA / SARIMA / SARIMAX / VAR, Holt-Winters, Prophet, walk-forward backtesting
- 🤖 **Machine Learning**: XGBoost, Ridge, Random Forest, LSTM, feature engineering, hyperparameter tuning
- 🔍 **Explainable AI**: SHAP explanations for individual predictions
- 🛡️ **Leakage-free pipelines**: time-based splits, look-ahead checks written as code
- 🖥️ **Interactive tools**: Streamlit apps and browser-based simulators
- 💻 **Problem Solving**: C++ and LeetCode

---

# 🔥 Featured Projects

## 🌫️ Next-Day Delhi AQI Forecast

Predicts **tomorrow's** air quality index for Delhi from **today's and past** air-quality and weather data, then explains every forecast with SHAP.

### 📊 Results

| Model | Test MAE (AQI points) |
| --- | ---: |
| "Tomorrow = today" baseline | 36.4 |
| **XGBoost** | **26.0** (28.6% lower) |

R² **0.91**, and the CPCB air-quality category is exactly right on **72%** of test days.

### 🔍 Highlights

- 56 features: pollutants, lags, rolling stats, hourly weather incl. boundary-layer height, stubble-burning season
- **Leakage checked by code**: every feature is rebuilt with the future deleted, for each of 2,009 days, and must not change
- Split on the date being *predicted*, not the feature date
- SHAP waterfall explanation for any single day
- COVID-19 lockdown case study: how a frozen model copes with a sudden regime shift
- 3-tab Streamlit app: explore a day, what-if analysis, model card

**Tech:** Python • Pandas • Scikit-learn • XGBoost • SHAP • Streamlit • Open-Meteo API

🔗 **Repository:**
https://github.com/anshulmittall/delhi-aqi-forecast

---

## 🛒 Demand Forecasting for Quick-Commerce Retail (M5 Walmart)

Forecasts the next **7 days** of daily FOODS sales for a Walmart store and measures how much better real models are than the simple replenishment rules used today.

### 📊 Results (52-week walk-forward test)

| Method | MAPE | RMSE (units) |
| --- | ---: | ---: |
| Past-week average rule (current practice) | 17.08% | 594.7 |
| Seasonal naive | 10.70% | 392.9 |
| SARIMAX | 7.84% | 299.2 |
| VARIMAX | 7.67% | 291.3 |
| **XGBoost** | **6.88%** | **254.7** |

**60% less error** than the current rule, and XGBoost wins in **50 of 52** test weeks.

### 🔍 Highlights

- **12 methods** compared on one identical walk-forward test (refit every week, never sees the future)
- Classical: Holt-Winters, ARIMA, SARIMA, plus ARIMAX / SARIMAX / VARIMAX with SNAP and event flags
- Advanced: Prophet, XGBoost, LSTM, tuned on a separate validation year
- Stationarity (ADF), ACF/PACF and AIC-based order selection
- Closure-aware forecasting: cleaning the 25 Dec closure cut the simple rules' Christmas-fortnight error by 38–40%
- Written up as an IEEE-format report

**Tech:** Python • Pandas • Statsmodels • Prophet • XGBoost • Keras (LSTM) • Matplotlib

🔗 **Repository:**
https://github.com/anshulmittall/quickcommerce-demand-forecast

---

# 📊 Other Projects

## 🔤 DFA / NFA String Processing Visualizer

An interactive simulator for automata theory: define your own **DFA, NFA or ε-NFA** and watch it process a string step by step.

- State diagram with active states and transitions highlighted at every step
- Play / pause / step controls with an input tape and a δ trace table (incl. ε-closures)
- Computation tree of every path an NFA can take
- Built-in test suite and input validation
- Runs entirely in the browser, with no install

**Tech:** JavaScript • HTML • CSS

🌐 **Live demo:** https://anshulmittall.github.io/dfa-nfa-visualizer/
🔗 **Repository:** https://github.com/anshulmittall/dfa-nfa-visualizer

---

## 💊 MediForecast AI: Medicine Demand Prediction System

A machine learning system that forecasts **medicine demand** from historical demand data and serves predictions through a web app.

- Random Forest regression model trained on historical demand
- Flask backend with an HTML frontend for real-time predictions

**Tech:** Python • Scikit-learn • Random Forest • Flask • HTML

---

# 💻 Data Structures & Algorithms

Practising problem solving in **C++** on LeetCode.

### 📚 Topics I'm Practising

`Arrays` • `Strings` • `Hashing` • `Two Pointers` • `Sliding Window` • `Recursion` • `Sorting` • `Binary Search` • `Linked Lists` • `Stacks` • `Queues` • `Trees` • `Graphs` • `Dynamic Programming`

🧩 **LeetCode:**
https://leetcode.com/u/auanshul/

🔗 **Solutions Repository:**
https://github.com/anshulmittall/leetcode

---

# 🛠️ Technical Skills

## 💻 Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

---

## 📊 Data Science & Machine Learning

![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-189FDD?style=for-the-badge)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-FF0D57?style=for-the-badge)

**Skills:** EDA • Feature Engineering • Regression • Hyperparameter Tuning • Cross-Validation • Model Evaluation • Explainability

---

## 📈 Time Series

![Statsmodels](https://img.shields.io/badge/Statsmodels-4051B5?style=for-the-badge)
![Prophet](https://img.shields.io/badge/Prophet-0668E1?style=for-the-badge&logo=meta&logoColor=white)

**Skills:** ARIMA • SARIMA • SARIMAX • VAR • Holt-Winters • LSTM • ADF Test • ACF/PACF • Walk-Forward Validation • RMSE / MAE / MAPE / WAPE

---

## 📉 Visualization & Apps

![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=for-the-badge&logo=matplotlib&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)

---

## ⚙️ Tools

![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![VS Code](https://img.shields.io/badge/VS%20Code-007ACC?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white)

**Skills:** Git • GitHub Pages • Virtual Environments • Reproducible Pipelines • Kaggle Datasets • REST APIs

---

# 🧠 Currently Working On

### 1. 📈 Time Series & Forecasting
Going deeper into forecasting models and how to evaluate them fairly.

### 2. 🔍 Explainable ML
Making model predictions understandable to the people who have to act on them.

### 3. 💻 Data Structures & Algorithms
Daily problem solving in C++ on LeetCode.

---

# 🏆 Achievements

- 🎓 **Dean's List, Semester 1**: awarded for a 9.72 SGPA
- 💡 **Smart India Hackathon 2025**: ranked in the Top 20 teams in the college-level internal round
- 🚀 **Participant**: Smart India Hackathon 2026, Microsoft Hackathon 2025

---

# 🤝 Let's Connect

I'm always happy to talk about **data, forecasting, ML, or interesting problems**, and open to collaborating on projects.

📧 **Email:**
anshulmttl123@gmail.com

💼 **LinkedIn:**
https://www.linkedin.com/in/auanshul/

🧩 **LeetCode:**
https://leetcode.com/u/auanshul/

🐙 **GitHub:**
https://github.com/anshulmittall
