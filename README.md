# 📉 Philosophy: A Fading Subject?  
### *Forecasting the future of academic interest using time series analysis*

---

## 📘 Overview  
Universities must constantly adjust course offerings and departmental resources based on shifting student interest. In this project, we explore whether **philosophy** is growing or declining in popularity — and what this means for university planning.

Using **Google Trends data from 2004–2015**, we analyze historical patterns in search interest for the term *“philosophy”* and build time series models to:

1. Forecast search popularity for 2016 and compare predictions to actual results  
2. Forecast search popularity for 2025  
3. Evaluate long-term interest and implications for universities

Our findings suggest a **clear downward trend**, with predicted 2025 values all below 50, indicating reduced public interest in philosophy as a subject.

---

## 🎯 Objectives  
- Understand trends and seasonality in search interest for “philosophy”  
- Fit an appropriate time series model (ARMA) for forecasting  
- Evaluate forecast performance using 2016 actual data  
- Predict monthly popularity values for 2025  
- Discuss implications for academic planning and resource allocation  

---

## 📊 Data Description  
- **Source:** Google Trends (`google.com/trends`)  
- **Variable:** Popularity index for the search term *“philosophy”*  
- **Scale:** 0–100 (100 = peak popularity)  
- **Time Range Used:** 2004–2015 for modeling  
- **Additional Years:** Actual 2016 values used for model validation  

---

## 🧪 Methods  
### **1. Exploratory Time Series Analysis**
- Identified long-term downward trend  
- Detected consistent seasonality — peaks at beginning and end of each year, dips during summer  
- Conducted trend extraction using moving averages  

### **2. Model Selection & Fitting**
- Fit multiple ARMA models to detrended data  
- Selected the best model using **AIC** (noting its tendency to favor more complex models)  
- Produced 12-month forecasts for 2016

### **3. Model Evaluation**
- Compared predictions to actual 2016 values  
- Errors were within **0–5 points**, indicating strong predictive performance  
- Detected smoothing effect from moving average trend extraction  

### **4. Forecasting for 2025**
- Generated monthly predictions assuming continuity of historical trend + seasonality  
- All predicted values were below 50, indicating declining long-term interest  

---

## 📈 Key Results  
### **Performance on 2016 Forecast**
- Predictions closely matched real values  
- Differences mostly between 0–5 points  
- Confirmed that ARMA captured core seasonal pattern  

### **2025 Forecast (Jan–Dec)**
39.99, 44.26, 42.53, 44.94, 38.88, 30.23,

27.80, 30.39, 41.61, 43.67, 44.42, 42.71


### **Interpretation**
- Popularity continues to decline  
- Seasonal pattern persists (winter peaks, summer dips)  
- Search interest remains below mid-range (50) for the entire year  
- Likely reflects reduced academic engagement with philosophy  

---

## 🧾 Discussion  
- **Trend extraction method matters:**  
  Moving averages introduced smoothing, making predicted changes milder than real fluctuations. Polynomial regression could capture more nuanced trends, but risks overfitting.

- **Model selection complexity:**  
  AIC may favor overly complex ARMA structures. BIC might produce simpler, more generalizable models.

- **Forecast uncertainty:**  
  Long-term predictions assume that past patterns persist. Real-world search behavior can shift due to cultural trends, academic policy, or technology.

- **Interpretation beyond numbers:**  
  Declining search interest may not imply declining relevance — discussions may be moving to social platforms, short-form content, or AI tools rather than traditional search.

---

## 🎓 Implications for Universities  
- Forecasts suggest **decreasing demand** for philosophy as a field of study  
- Possible need to:
  - Reduce course offerings  
  - Scale down program size  
  - Reallocate instructional resources  
- Universities should monitor future trend shifts but consider diversification or interdisciplinary approaches (e.g., philosophy + AI ethics)

---

## 🔧 Tech & Tools  
**Languages:** R 
**Time Series Tools:** ARMA/ARIMA, moving averages, AIC  
**Plots & Analysis:** ggplot2 
**Data Source:** Google Trends  

---

