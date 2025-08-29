# Terrestrial Ionosphere Modelling

This project models the terrestrial ionosphere, an environment that strongly influences modern satellite communication systems. The analysis uses electron density profiles from ESA’s SPENVIS portal and compares them with the hydrogen 2s orbital probability equation. The goal is to study the structure of the ionosphere and see how well this atomic orbital function can approximate real ionospheric data. This was my second project under the supervision of Prof. Iver Cairns (USYD) as part of the Physics Special Studies Program at USYD.

The **electron density** is the key property of interest, and the notebook is divided into two main sections:

1. **SPENVIS Data Exploration**  
   - Extracts ionosphere data from ESA’s [SPENVIS](https://www.spenvis.oma.be/) portal.  
   - Graphs zenith electron density profiles over four antipodal locations around the globe.  
   - Provides a simple demonstration of commonalities and differences in the ionosphere across Earth.

2. **Hydrogen Orbital Fitting**  
   - Optimises the hydrogen 2s orbital electron probability function to fit real ionospheric electron density data.  
   - Motivated by the resemblance of the 2s orbital profile to the idealised ionospheric electron density profile.  
   - Uses non-linear least squares and Nelder–Mead methods.  
   - Quality of fits assessed using residual plots.

## Folder Structure
- `src/TECmodel.ipynb` — main notebook with analysis and visualisations.  
- `data/` — SPENVIS ionosphere data files.  

## Requirements
- Python 3.10+  
- Jupyter Notebook  
- numpy, matplotlib, scipy, pandas  

Install with:
```bash
pip install numpy matplotlib scipy pandas jupyter
```

## Usage
1. Place SPENVIS data files into the `data/` folder.  
2. Launch Jupyter and open the notebook:  
   ```bash
   jupyter notebook src/TECmodel.ipynb
   ```  
3. Run all cells to reproduce the analysis and plots.  

## Author
Developed by **Yunki Yau**  
GitHub: [yunkiyau](https://github.com/yunkiyau)  
Email: yunki.yau@gmail.com  

## Acknowledgements
Supervised by Prof. Iver Cairns - USYD Professor of Space Physics, Director, CUAVA: the ARC Training Centre for CubeSats, UAVs, and Their Applications.
