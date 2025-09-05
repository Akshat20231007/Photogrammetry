# Photogrammetry using Microsoft AirSim & Agisoft Metashape

This project demonstrates a **virtual photogrammetry workflow** using the [Microsoft AirSim](https://github.com/microsoft/AirSim) drone simulator.  
A virtual survey of the **Neighbourhood environment** was conducted using simulated drones, images were captured, and a **3D reconstruction** was performed using **Agisoft Metashape**.

---

## 🚀 Project Workflow
1. **Drone Simulation with AirSim**
   - Configured multiple drones in `settings.json`.
   - Implemented **angled survey** (`AngledSurvey.py`) and **vertical survey** (`VerticalSurvey.py`) scripts for autonomous flight and image capture.

2. **Image Capture**
   - Drones follow predefined flight paths.
   - Capture high-resolution RGB images at intervals.
   - Store images in local directories.

3. **3D Reconstruction**
   - Captured images were imported into **Agisoft Metashape**.
   - Generated a **3D point cloud, textured mesh, and DEM** of the environment.

---

## 📂 Files
- `settings.json` → AirSim configuration (multiple drones setup).
- `AngledSurvey.py` → Multi-drone angled photogrammetry survey.
- `VerticalSurvey.py` → Multi-drone vertical photogrammetry survey.
- `requirements.txt` → Python dependencies.
- `results/` → (optional) Sample images or reconstructed models.

---

## 🛠️ Requirements
- Python 3.8+
- [Microsoft AirSim](https://github.com/microsoft/AirSim) (with Neighbourhood environment)
- [Agisoft Metashape](https://www.agisoft.com/) (for reconstruction)
- Python packages:
  ```bash
  pip install -r requirements.txt
  ```

---

## ▶️ Running the Simulation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/photogrammetry-airsim
   cd photogrammetry-airsim
   ```

2. Start the AirSim Neighbourhood environment.

3. Run the survey script:
   ```bash
   python AngledSurvey.py
   ```
   or
   ```bash
   python VerticalSurvey.py
   ```

4. The captured images will be saved in the working directory.

5. Import the images into **Agisoft Metashape** (or any photogrammetry tool) to generate the 3D model.

---

## 📸 Results
- 3D point cloud
- Textured mesh
- DEM (Digital Elevation Model)

---

## ✨ Credits
- [Microsoft AirSim](https://github.com/microsoft/AirSim)
- [Agisoft Metashape](https://www.agisoft.com/)
