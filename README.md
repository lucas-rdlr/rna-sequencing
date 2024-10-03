## Table of contents
* [General info](#general-info)
* [Instalation](#instalation)
* [Outline](#outline)

# General info

This repository aims to serve as a tutorial for common single cell RNA sequencing data processing and analysis. It gives an insight intothe pre-processing step along with the quality control metrics. Finally, it shows a practical example applying it to compare the performance of common imputation methods in bioinformatics (technically clearance or denoising methods in mathemtatics).

# Instalation

The repository uses widely known python packages for the preprocessing, mainly pandas and scanpy and a `src` folder has been added containing the algorithms for the imputation methods. For the "Sinkhorn" algorithm (last practical part of the tutorail) a GPU is quite neccesary since the Optimal Transport algorithms require a large ammount of memory. For the pre-processing steps a CPU should be more than enough. To correctly run the code, I suggest using a virtual environment (not neccesarly conda) to avoid version compatibilities.<br>

Clone the repository by doing:
```
git clone 

```
python -m venv [path to environment]
```

Activate the environment before installing dependencies. In Linux:
```
source [path to environment]/bin/activate
```

Lastly, you can 

# Outline

 - `src` contatins all the `.py` modules including datasets and training functions.
 - `notebooks` contains the `.ipynb` files with the experiments and tested functions.
 - `requirements.txt` the virtual environment file which can be used to install packages.

# Folder structure
```
├── data
│   ├── external
│   └── internal
├── experiments
├── models
├── notebooks
│   ├── data_science_bowl_2018.ipynb
│   ├── DeepLab.ipynb
│   ├── draft.ipynb
│   ├── general.ipynb
│   ├── __init__.py
│   ├── MaskRCNN.ipynb
│   ├── mesh_alice.ipynb
│   ├── prueba.py
│   ├── tracking.ipynb
│   └── UNet.ipynb
├── README.md
├── requirements.txt
├── src
│   ├── data
│   ├── datasets.py
│   ├── downloads.py
│   ├── features
│   ├── initializer.py
│   ├── __init__.py
│   ├── labeling.py
│   ├── models
│   ├── nets.py
│   ├── processing.py
│   ├── __pycache__
│   ├── segmentation.py
│   ├── training.py
│   ├── transformations.py
│   ├── visualization
│   └── visualization.py
└── tree.txt

```
