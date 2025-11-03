# Local-Network-Temperature-Humidity-Dashboard


## 🧠 ML Features Implemented

### 1️⃣ Predictive Analytics
- **Linear Regression** for temperature & humidity trends  
- **1-hour ahead predictions** based on historical patterns  
- **Trend visualization** → Rising 📈 / Falling 📉 / Stable ⚖️  

### 2️⃣ Anomaly Detection
- **Z-score method** to detect unusual spikes  
- **Alerts** when readings deviate > **2.5 standard deviations**  
- **Real-time notifications** for anomalies ⚠️  

### 3️⃣ Comfort Index Algorithm
- **Heat Index calculation** (feels-like temperature)  
- **Optimal range analysis**: 20–26 °C temperature, 40–60 % humidity  
- **Visual Comfort Score (0–100)** displayed as a **color-coded bar** 🌈  

### 4️⃣ Statistical Analysis
- **Running mean** & **standard deviation**  
- **Data collection:** last 100 samples stored  
- **Pattern recognition** over time for adaptive insights  

---

## ⚙️ How It Works

### 🧩 Data Collection
- Samples taken **every 2 seconds**  
- Maintains a **rolling window** of **100 most recent readings**  
- Starts analysis once **10+ samples** are available  

### 🤖 ML Algorithms
- **Linear Regression:** calculates rate of change for temp/humidity  
- **Z-Score Detection:** automatically identifies outliers  
- **Comfort Scoring:** multi-factor evaluation of environmental comfort  

### 🔮 Predictions
- Uses **trend slopes** to forecast **1 hour ahead**  
- Updates in **real-time** as new data arrives  
- Accuracy improves after **20+ samples**  

---

## 📊 What You’ll See
| Feature | Description |
|----------|--------------|
| 📈 **Trends** | Real-time temperature/humidity rate (e.g., +0.5 °C/hour) |
| 🔮 **Predictions** | 1-hour ahead forecast |
| ⚠️ **Anomalies** | Alerts for abnormal spikes |
| 😊 **Comfort Score** | 0–100 visual score bar |
| 📊 **Statistics** | Mean, Std. Dev., and total samples |

💡 The ML runs **entirely on the ESP32 — no cloud required!**  
It learns from your environment and alerts you to unusual conditions automatically.

---

## 📶 How to Connect

1. **Turn on your phone’s hotspot**  
   - **SSID:** `circuitX`  
   - **Password:** `1029384756`  

2. **Connect your viewing device** (phone/laptop) to the same hotspot.  
3. Ensure **2 devices** are connected:  
   - ✅ ESP32  
   - ✅ Dashboard viewing device  

---

### 🌐 Access Dashboard

```bash
http://10.49.99.100
