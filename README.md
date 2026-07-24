# Measurement and Analysis of Zebrafish Behavior Tutorial

Welcome to the **Zebrafish Social Behavior Tutorial** repository. This tutorial provides an interactive guide to analyzing an organism-scale social behavior.

---

## Overview
In this two-day lab practice, we will use a Jupyter notebook (which will be provided) to visualize the 3D trajectories of two swimming adult zebrafish and learn how to interact with the data to extract interpretable behavioral insights.

---

## Installation & Local Setup

## Prerequisites: Install Miniconda & Setup Jupyter

If you do not have Conda installed, please follow these steps to set up your environment on MacOS, etc.

### 1. Download the Installer
Open your terminal and run the command that matches your Mac's processor:

* **For MacOS (M1/M2/M3/M4 chips):**
```bash
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh
```
* **For MacOS (intel-based):**
```bash
curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
```

* **For 64-bit Windows:**
```cmd
curl -L -o miniconda_installer.exe [https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.sh](https://repo.anaconda.com/miniconda/Miniconda3-latest-Windows-x86_64.sh)
```
 
### 2. Run the Installer Script
Execute the installer you just downloaded:

* **For Apple Silicon (M1/M2/M3/M4 chips):**
```bash
bash Miniconda3-latest-MacOSX-arm64.sh
```
* **For Intel-based MacOS:**
```bash
bash Miniconda3-latest-MacOSX-x86_64.sh
```

* **For 64-bit Windows:**
```text
simply double-click the .exe file to launch the standard Windows installation wizard.
```

### 3. Follow the Prompts
Press Return to review the license agreement, then type yes to agree.
Press Return to accept the default installation location.
When asked to initialize Miniconda, type yes. This allows the conda command to work natively in your terminal.

### 4. Refresh Your Terminal
Apply the changes to your terminal immediately by reloading your shell configuration:
* **macOS :**
```bash
source ~/.zshrc
```
* **macOS or Windows:**
Alternatively, close your current terminal window and open a new one.

### 5. Create Folder and Save Configuration
Manual Steps:
1. Open your file manager (File Explore on Windows or Finder on macOS)
2. Navigate to your desired location (for example, inside of Documents or Desktop)
3. Create a new folder (for example, 2fish_tutorial)
4. Save the environment.yml inside this new folder

### 6. Change your terminal's directory to the new folder (e.g. 2fish_tutorial) using the cd command.
* **macOS (use Terminal):**
```bash
cd ~/Documents/2fish_tutorial
```
* **Windows (use Anaconda Prompt):**
```bash
cd C:\Users\YourUsername\Documents\2fish_tutorial
```

### 7. Create and Activate the Environment
Create the Conda Environment
Build the project environment using the provided configurations:
```bash
conda env create -n 2fish_tutorial -f environment.yml
```

### 8. Activate the Environment
Activate your new isolated workspace:
```bash
conda activate 2fish_tutorial
```

### 9. Install Jupyter Notebook
```bash
conda install -c conda-forge notebook -y
```

### 10. Launch the Tutorial
Fire up the local host server to begin:
```bash
jupyter notebook
```
---

## Running in the Cloud (No Installation Required)

If you prefer not to install anything locally, you are welcome to try Binder (https://mybinder.org/), Google CoLab (https://colab.research.google.com/), or something similar.

---
## References
 
> Zebrafish Dataset:
> * Deligkaris, K., Neiman, R., Hiroi, M., Izawa, T., O’Shaughnessy, L., Rodriguez, L. C., Masai, I., & Stephens, G. J. (2026). A dataset of fine-grained zebrafish interactions in health and disease. Scientific Data, 13(1), 583. https://doi.org/10.1038/s41597-026-06953-6 
>
> Analysis of Zebrafish Fighting:
> * O'Shaughnessy, L., Izawa, T., Masai, I., Shaevitz, J. W., & Stephens, G. J. (2024). Dynamics of Dominance in Interacting Zebrafish. PRX Life, 2(4), 043006. https://doi.org/10.1103/PRXLife.2.043006
> * Kawano, A., O’Shaughnessy, L., Neiman, R., Deligkaris, K., Rodriguez, L. C., Masai, I., & Stephens, G. J. (2025). Decomposing Predictive Information in Social Dynamics. bioRxiv, 2025.2005.2016.654393. https://doi.org/10.1101/2025.05.16.654393 
---

## Acknowledgements

Thanks: Mariia Pavelchenko and Luis Carretero
