# ☀️ HelioScope
**Smarter solar, measured in real carbon.**

HelioScope is a localized rooftop solar and grid displacement forecaster that demonstrates how geographical placement directly dictates the real-world climate impact of solar installations. 

Built for **Lake Oswego Hacks 2026**.

## 🌍 The Core Insight: Generation vs. Displacement
Standard calculators focus on financial savings and raw energy generation. HelioScope focuses on **carbon displacement**. 

Generating 1 kWh of solar power in a clean-energy grid (like the US Pacific Northwest) mostly displaces existing clean hydro power. However, generating that exact same 1 kWh in a coal-heavy grid (like Eastern India) is a massive win for the planet because it directly stops a fossil-fuel plant from burning coal. 

Our model visualizes this disparity. For a standard 40 m² residential rooftop:
* **Portland, OR Baseline:** Offsets ≈190 kg of CO₂ per month.
* **Kolkata, India Contrast:** Offsets ≈753 kg of CO₂ per month (**Nearly 4× the climate impact**).

## ⚙️ Tech Stack
* **Backend Engine:** Python 3
* **Frontend UI:** Gradio
* **Data Visualization:** Matplotlib
* **Environment:** Google Colab
* **Data Sources:** U.S. EPA eGRID, India Central Electricity Authority, NREL PVWatts

## 🚀 How to Run the App
Because HelioScope was built for rapid prototyping and accessibility, the entire application runs directly in your browser via Google Colab without needing local installation.

1. Open the `HelioScope.ipynb` file in this repository.
2. Click the blue **"Open in Colab"** badge at the top of the file viewing window.
3. In Google Colab, click **Runtime > Run all** in the top menu bar to install dependencies and execute the engine.
4. Scroll to the bottom of the notebook and click the public **Gradio web link** (`https://[random-string].gradio.live`) to use the interactive dashboard.

## 🔮 Future Roadmap
* **Global API Integration:** Connecting Geopy, the ElectricityMaps API, and NASA POWER to allow users to fetch live regional irradiance and grid carbon baselines via local postal code.
* **Computer Vision Roof Detection:** Integrating satellite imagery APIs to calculate usable roof area automatically rather than relying on manual user inputs.
