# 📈 Casey Clean Overlay (TradingView)

A clean, professional TradingView indicator inspired by Casey-style intraday trading.

<img width="2477" height="1154" alt="image" src="https://github.com/user-attachments/assets/ed25442f-024f-4cbb-9bae-cdf68334d1d1" />


This script focuses on:
- **Key price levels (PDH / PDL / PMH / PML)**
- **Trend structure (EMA 13 / 48 / 200)**
- **Institutional bias (VWAP)**
- **Actionable trade signals (CALL / PUT arrows)**

Designed for **clarity, simplicity, and real trading use**.

---

## 🚀 Features

### 🎯 Core Levels (Always Horizontal)
- **PDH (Previous Day High)** — solid blue
- **PDL (Previous Day Low)** — solid blue
- **PMH (Premarket High)** — dashed orange
- **PML (Premarket Low)** — dashed orange

✅ Flat horizontal lines (no bends)  
✅ Only shown for the **current trading day**  
✅ Automatically reset each new day  

---

### 📊 Technical Indicators (Toggleable)
- **EMA 13 (yellow)** — short-term momentum
- **EMA 48 (purple)** — mid-term trend
- **EMA 200 (red)** — overall trend bias
- **VWAP (aqua)** — institutional reference

✅ Can be turned ON/OFF individually  
✅ Values appear in the **top-left legend (like built-in indicators)**  

---

### 🏷 Right-Edge Labels
- PDH / PDL / PMH / PML labels on the **far right of the chart**
- Always aligned with their price levels
- Update in real time

---

### 🟢🔴 Trade Signals (Casey-style)
Thin arrows indicate potential trade opportunities:

#### 🟢 CALL (Bullish)
- PDH breakout  
- PDL bounce  
- PMH breakout (secondary)  
- EMA13 pullback continuation  

#### 🔴 PUT (Bearish)
- PDH rejection  
- PDL breakdown  
- PML breakdown (secondary)  
- EMA13 rejection continuation  

---

### 💬 Hover Explanations (Unique Feature)
Each signal includes a nearby **`?` marker**:

👉 Hover over the `?` to see:
- Why the signal triggered
- Which level or condition caused it

> ⚠️ Note: TradingView does **not support tooltips on arrows**, so the `?` marker is required.

---

### 🧠 Built-In Trading Logic

The script follows this decision flow:

1. **Identify key level interaction**
   - Breakout
   - Rejection
   - Bounce

2. **Confirm trend**
   - EMA alignment (13 / 48 / 200)

3. **Confirm bias**
   - Above VWAP → bullish  
   - Below VWAP → bearish  

4. **Entry trigger**
   - Immediate level reaction  
   - OR EMA13 pullback continuation  

---

## 📌 Best Use Case

- Designed for **intraday trading**
- Works best on:
  - **2-minute chart (recommended)**
  - 1–5 minute timeframes

---

## ⚠️ Limitations

- This is **not a full automation of Casey’s discretionary system**
- Does NOT include:
  - Flag pattern recognition
  - Volume confirmation
  - Multi-timeframe analysis

👉 Treat signals as **decision support**, not blind entries

---

## 🛠 Installation (TradingView)

### Step 1 — Open Pine Editor
1. Go to **https://www.tradingview.com/**
2. Open any chart
3. Click **“Pine Editor”** at the bottom

---

### Step 2 — Add Script
1. Delete any existing code
2. Paste the full script into the editor

---

### Step 3 — Save & Add to Chart
1. Click **“Save”**
2. Click **“Add to Chart”**

---

### Step 4 — Enable Extended Hours (IMPORTANT)
To see **PMH / PML**:

1. Click the gear icon ⚙️ on chart
2. Go to **Symbol**
3. Enable: 
---

### Step 5 — Configure Settings
Click the indicator settings and customize:

- Toggle EMAs / VWAP
- Toggle signals
- Toggle hover explanations
- Toggle right-side labels

---

## 🎨 Visual Design Philosophy

- Minimal clutter
- Clear level hierarchy:
- **Blue = major levels (PDH/PDL)**
- **Orange = secondary levels (PMH/PML)**
- Thin arrows for clean execution view
- Optional contextual overlays

---

## 🔥 Pro Tips

- Best setups:
- **PDH rejection → PUT**
- **PDL bounce → CALL**
- **EMA13 pullback in strong trend**

- Avoid trading:
- Inside PMH/PML range (chop zone)

- Combine with:
- Volume spikes
- Opening range breakouts

---

## 📜 Disclaimer

This script is for **educational purposes only**.

Trading involves risk.  
Do not trade real money without proper risk management.

---

## 👨‍💻 Author Notes

This script was designed to:
- Replace manual drawing of levels
- Provide structure for discretionary trading
- Stay visually clean and intuitive

---

## ⭐ Future Enhancements (Optional)

- A+ signal filtering (higher probability only)
- Flag pattern detection
- Opening range logic
- Volume confirmation

---
