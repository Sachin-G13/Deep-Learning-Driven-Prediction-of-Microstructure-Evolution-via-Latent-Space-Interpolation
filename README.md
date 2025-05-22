# 📘 Deep Learning-Driven Prediction of Microstructure Evolution

This repository provides the complete implementation of the paper:

**_Deep Learning-Driven Prediction of Microstructure Evolution via Latent Space Interpolation_**  
*Sachin Gaikwad, Thejas Kasilingam, Owais Ahmad, Rajdip Mukherjee, Somnath Bhowmick*  
📅 *Dated: May 22, 2025*

---

## 📌 Overview

This project demonstrates a deep generative modeling approach to predict and visualize the time evolution of microstructures in binary alloys across different composition values. It leverages:

- A **Conditional Variational Autoencoder (CVAE)** to model the latent space of microstructure images.
- **Cubic Spline Interpolation** to generate intermediate phase labels.
- **Spherical Linear Interpolation (SLERP)** to ensure smooth morphological transitions between microstructures.

The model replicates the temporal and spatial evolution of microstructures as observed in traditional phase-field simulations, but at a fraction of the computational cost.

---

## 📁 Repository Structure

```
.
├── model_training.ipynb        # Training the CVAE model
├── model_prediction.ipynb      # Generating intermediate microstructures using cubic and SLERP interpolation
├── model_analysis.ipynb        # Autocorrelation and timestep vs. average area comparison
├── utils.py                    # Utility functions used across notebooks
├── data/                       # (Optional) Place for data or instructions on how to obtain it
└── README.md                   # This file
```

---

## 🧠 Key Techniques

- **Conditional VAE** for learning latent space representations of microstructures.
- **Cubic Spline Interpolation** for generating interpolated phase labels between known composition values.
- **SLERP** in the latent space for producing temporally smooth microstructure evolution sequences.
- **Morphological Validation** using:
  - Timestep vs. average white area plots
  - 2-point autocorrelation function comparison

---

## 🔗 Downloads

- 📦 [Download Dataset (Google Drive)](https://drive.google.com/file/d/1jFUpb0h06S6UcLUq5QBRcL4o7xlYnep2/view?usp=sharing)
- 💾 [Download Pretrained CVAE Weights](https://drive.google.com/file/d/18J1Z4myVTj0tv3vE1LjYe2OusPseJurP/view?usp=sharing)

---

## ▶️ How to Run

1. **Clone this repository**:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   cd <repo-name>
   ```

2. **Install required dependencies**:
   ```bash
   pip install -r requirements.txt  # if you provide one
   ```

3. **Run notebooks in order**:
   - `model_training.ipynb` → Train the CVAE
   - `model_prediction.ipynb` → Generate new microstructures
   - `model_analysis.ipynb` → Visualize and validate results

---

## 📄 Citation

If you use this work, please cite:

> **Gaikwad, S., Kasilingam, T., Ahmad, O., Mukherjee, R., & Bhowmick, S. (2025)**.  
> Deep Learning-Driven Prediction of Microstructure Evolution via Latent Space Interpolation.  
> _Indian Institute of Technology (BHU) & IIT Kanpur._

---

## 📧 Contact

- Somnath Bhowmick – *bsomnath@iitk.ac.in* (corresponding author)
