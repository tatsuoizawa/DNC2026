# Measurement and Analysis of Zebrafish Behavior Tutorial

Welcome to the **Zebrafish Social Behavior Tutorial** repository. This tutorial provides an interactive guide to analyzing an organism-scale social behavior.

---

## Citation
If you find this tutorial, algorithms, or datasets useful in your research, please cite:

> This Tutorial: Izawa, T. (2026). *Measurement and Analysis of Zebrafish Social Behavior: A Hands-on Tutorial Series*. Zenodo. https://doi.org/xx.xxxx/zenodo.xxxxxxx
> 
> Zebrafish Dataset: Deligkaris, K., Neiman, R., Hiroi, M., Izawa, T., O’Shaughnessy, L., Rodriguez, L. C., Masai, I., & Stephens, G. J. (2026). A dataset of fine-grained zebrafish interactions in health and disease. Scientific Data, 13(1), 583. https://doi.org/10.1038/s41597-026-06953-6 
>
> Analysis of Zebrafish Fighting: O'Shaughnessy, L., Izawa, T., Masai, I., Shaevitz, J. W., & Stephens, G. J. (2024). Dynamics of Dominance in Interacting Zebrafish. PRX Life, 2(4), 043006. https://doi.org/10.1103/PRXLife.2.043006

---

## Overview of the Tutorials
In this tutorial, we will use this notebook to visualize the 3D trajectories of two swimming adult zebrafish and interact with the trajectory data. The required data - along with optional raw videos - will be provided on a flash drive (~30GB). To analyze the data, we will use these trajectories to calculate the distance between the two fish, their individual speeds, and their interactions (approach and escape behavior). If time permits, we will discuss additional parameters we can compute to extract interpretable behavioral insights.

---

## Installation & Local Setup

## Prerequisites: Install Miniconda & Setup Jupyter

If you do not have Conda installed, please follow these steps to set up your environment on macOS.

### 1. Download the Installer
Open your terminal and run the command that matches your Mac's processor:

* **For Apple Silicon (M1/M2/M3/M4 chips):**
```bash
  curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-arm64.sh
```
* **For Intel:**
```bash
  curl -O https://repo.anaconda.com/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
```
### 2. Run the Installer Script
Execute the installer you just downloaded:

* **For Apple Silicon (M1/M2/M3/M4 chips):**
bash Miniconda3-latest-MacOSX-arm64.sh
* **For Intel:**
bash Miniconda3-latest-MacOSX-x86_64.sh

### 3. Follow the Prompts
Press Return to review the license agreement, then type yes to agree.
Press Return to accept the default installation location.
When asked to initialize Miniconda, type yes. This allows the conda command to work natively in your terminal.

### 4. Refresh Your Terminal
Apply the changes to your terminal immediately by reloading your shell configuration:
source ~/.zshrc

(Alternatively, close your current terminal window and open a new one).

### 5. Create and Activate the Environment
Create the Conda Environment
Build the project environment using the provided configurations:
conda env create -n 2fish_tutorial -f environment.yml

### 6. Activate the Environment
Activate your new isolated workspace:
conda activate 2fish_tutorial

### 7. Install Jupyter Notebook
If Jupyter Notebook is not already included in your environment.yml file, manually add it to the active workspace by running:
conda install -c conda-forge notebook -y

### 8. Launch the Tutorial
Fire up the local host server to begin:
jupyter notebook

---

## Running in the Cloud (No Installation Required)

If you prefer not to install anything locally, you are welcome to try Binder (https://mybinder.org/), Google CoLab (https://colab.research.google.com/), or something similar.

---

## Contributors & Acknowledgements
