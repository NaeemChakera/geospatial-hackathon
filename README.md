# Geospatial Python Crash Course 
The following jupyter notebooks have been adapted from the Carpentries material [Introduction to Geospatial Raster and Vector Data with Python](https://carpentries-incubator.github.io/geospatial-python/).



These notebooks are designed to extend your skills through applied examples. A foundational understanding of geospatial data concepts is assumed. If you’re new to the topic, you should review Episodes 1–4 of the Carpentries lesson before working through this content.


A [Comprehensive GIS Primer](geospatial_primer.pdf) has also been developed, featuring curated resources and further reading. In addition to the materials listed below, the following GitHub repository provides ESRI-specific guidance and tutorials:
https://github.com/tgiles-esri/CSU-Hackathon-Esri-Resources

Notebooks included
- **usda_quickstats.ipynb** – Explore and map agricultural data using the USDA Quick Stats API
- **naip.ipynb** – Access and work with NAIP imagery for analysis and model training
- **landsat_merge.ipynb** – Merge and process Landsat imagery using averaging techniques

## Setup Guide

This guide walks you through setting up your local environment to run the **Geospatial Python Crash Course** repository.

---

## 1. Open the Command Line

### **Windows**

* Press `Win + S` and search for **Command Prompt** or **PowerShell**
* Click to open
  *(Recommended: use **Anaconda Prompt** if you already have Anaconda installed)*

### **Mac**

* Press `Cmd + Space` to open Spotlight Search
* Type **Terminal** and press Enter

---

## 2. Clone the Repository

Navigate to the directory where you want the project stored, then run:

```bash
git clone https://github.com/GeospatialCentroid/geospatial-python-crash-course.git
cd geospatial-python-crash-course
```

---

## 3. Install Conda (conda-forge)

If you **do not already have Conda installed**, install **Miniconda**:

### Download Miniconda

* https://docs.conda.io/en/latest/miniconda.html

Follow the installer instructions for your operating system.

---

### Configure conda-forge (recommended)

After installation, open a new terminal and run:

```bash
conda config --add channels conda-forge
conda config --set channel_priority strict
```

---

## 4. Create the Environment from `environment.yml`

Inside the cloned repository folder, run:

```bash
conda env create -f environment.yml
```

This will create a new environment with all required dependencies.

---

## 5. Activate the Environment

```bash
conda activate geospatial-python-crash-course
```

*(If the environment name differs, check `environment.yml` for the exact name.)*

---

## 6. Launch Jupyter Notebook

Start Jupyter Notebook with:

```bash
jupyter notebook
```

This will open a browser window. From there:

* Navigate to the project folder
* Open any `.ipynb` notebook to begin

---

## Troubleshooting Tips

* If `conda` is not recognized:

  * Restart your terminal
  * Ensure Conda was added to your system PATH during installation

* If environment creation fails:

  * Try updating conda:

    ```bash
    conda update -n base -c defaults conda
    ```

* If Jupyter does not open automatically:

  * Copy and paste the provided URL into your browser

---

## You're Ready!

You should now be able to run all notebooks in the repository and follow along with the crash course.
