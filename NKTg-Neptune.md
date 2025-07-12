# NKTg-Law-Simulation: Predicting Planetary Motion with NASA Data and Python

This repository applies the **NKTg Law** — a new motion model that considers mass variation — to simulate the orbital behavior of Neptune using real NASA data from 2023. The simulation predicts Neptune’s 2024 motion **with near-zero error**, showing the effectiveness of the NKTg framework.

---

## 🚀 Project Overview

Traditional mechanics often treat mass as constant. But in reality, gas giants like Neptune slowly lose mass over time (e.g., hydrogen escape). The **NKTg Law** accounts for this, enabling reverse and forward motion predictions based on two conserved quantities:

- **NKTg₁ = x × p**  
- **NKTg₂ = (dm/dt) × p**

Where:
- `x`: position  
- `v`: velocity  
- `m`: mass  
- `p = m × v`: momentum  
- `dm/dt`: rate of mass change

---

## 📊 Input Data

- Source: [NASA JPL Horizons](https://ssd.jpl.nasa.gov/horizons)
- Neptune’s orbital data for 2023 (position, velocity, mass)
- Assumed gas loss rate: `–0.00002000 kg/s`

---

## 📐 How the Model Works

1. From 2023 NASA data, compute:
   - `p = m × v`
   - `NKTg₁ = x × p`
   - `NKTg₂ = (dm/dt) × p`
2. Assume new `m` for 2024
3. Recalculate:
   - `p = m_new × v`
   - `x = NKTg₁ / p`

---

## 🐍 Python Example

```python
# Constants
NKTg1 = 2.503e36     # From 2023 data
velocity = 5.43      # km/s
mass_2024 = 1.024299e26  # Adjusted for gas loss

# Simulation
p = mass_2024 * velocity
x = NKTg1 / p
print(f"Predicted position (km): {x:.3e}")
✅ Results
Date	NASA x (km)	NKTg x (km)	Error	Notes
2024-01-01	4.498e+9	4.498e+9	~0 km	Perfect match
2024-07-01	4.553e+9	4.553e+9	~0 km	Perfect match
2024-12-31	4.498e+9	4.498e+9	~0 km	Perfect match

✔️ Position and velocity match NASA data
✔️ Mass deviation consistent with gas loss model (~0.000020%)

📂 Repository Contents
nktg_simulation.py: Python simulation script

NKTg_Neptune_2023_2024_Data.xlsx: Real and simulated data

README.md: Project explanation

/results/: Output comparisons and charts

📚 References
NASA JPL Horizons

Neptune Factsheet (NASA)

Hydrogen Escape on Neptune (Nature)

🧠 Future Work
Extend to Uranus, Saturn, or comets

Qt GUI for real-time visualization

Connect to satellite systems with dynamic mass (fuel loss, ejection)

👤 Author
Nguyen Khanh Tung
📧 traiphieu.com@gmail.com
🌐 https://traiphieu.com
🆔 ORCID: 0009-0002-9877-4137
