# 🏗️ Solar System Simulation  

## 📜 Overview  
This project simulates the **orbits of planets in the solar system** and calculates the **average closest planet to Earth** over a 1000-year period. The simulation assumes **perfectly circular orbits**, all lying on the same plane, and calculates **planetary positions** using trigonometric functions.  

## 🎯 Problem Explanation  
The simulation models planetary motion using the following components:  

1. **Planet Class**  
   - Each planet is represented by a **radius (orbital distance)** and **year length (days per orbit)**.  
   - The `position(day)` function computes the planet’s **x, y coordinates** at any given day using trigonometry (`sohcahtoa`).  

2. **Distance Calculation**  
   - Computes the **Euclidean distance** between two planets on a specific day.  

3. **Closest Planet Simulation**  
   - Runs for **1000 Earth years** (365,000 days).  
   - Computes the **average distance** between all planet pairs over this period.  
   - Determines which planet is **closest to Earth on average**.  

4. **Time-Series Analysis**  
   - Runs an additional **1000-day simulation** storing the daily distance from Earth to Mercury, Venus, and Mars.  
   - Uses **Pandas and Matplotlib** to visualize these distances over time.  

## 🛠️ Implementation Details  
- **Planetary Positioning:**  
  - Uses circular orbits and trigonometry to determine `(x, y)` coordinates.  
- **Distance Computation:**  
  - Uses the formula:  
    ```python
    distance = sqrt((x2 - x1)**2 + (y2 - y1)**2)
    ```
- **Efficiency Considerations:**  
  - Discusses whether **random sampling** would improve simulation speed.  
