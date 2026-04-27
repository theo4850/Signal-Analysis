# 📡 Hydrogen Line Detection from Noisy Radio Signals

> End-to-end signal processing pipeline for detecting weak spectral signals in noisy data.

---

## 🚀 Project Highlights

* 🔬 Simulated realistic radio astronomy signals
* 📉 Reduced noise using averaging and smoothing
* ⚙️ Applied ON/OFF calibration to remove background
* 📊 Detected spectral line using SNR analysis
* 🔍 Improved resolution via interpolation
* 📐 Performed Gaussian fitting
* 📈 Evaluated accuracy using ground truth
* 🧪 Compared multiple signal processing approaches

---

## 🎯 Key Result

The alternative pipeline achieved **dramatically lower error**:

* MSE reduced by more than **100×**
* Much more accurate reconstruction of the spectral line

---

## 📊 Example Output

✔ Clean detection of the hydrogen line at 1420 MHz
✔ Accurate Gaussian fit
✔ Clear improvement after smoothing and interpolation

*(See notebook for full visualizations)*

---

## ⚙️ Methodology

### Signal Model

OFF = background + noise
ON = background + noise + spectral line

---

### Calibration

calibrated = ON / OFF

Removes background and highlights the signal of interest.

---

### Processing Steps

1. Averaging → noise reduction
2. Smoothing → cleaner signal
3. SNR analysis → detect signal region
4. Interpolation → increase resolution
5. Gaussian fitting → model spectral line

---

## 🔁 Alternative Approach

Tested a second pipeline using:

* Savitzky-Golay smoothing
* Cubic interpolation
* Different noise model

👉 Result: **significant accuracy improvement**

---

## 🛠️ Tech Stack

* Python
* NumPy / SciPy
* Matplotlib
* Pandas

---

## 📂 Structure

```
notebooks/Analysis.ipynb
```

---

## ▶️ Run the Project

Open the notebook and run all cells:

```
notebooks/Analysis.ipynb
```
