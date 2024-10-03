## Table of contents
* [General info](#general-info)
* [Installation](#installation)
* [Outline](#outline)

# General info

This repository aims to serve as a tutorial for common single cell RNA sequencing data processing and analysis. It gives an insight intothe pre-processing step along with the quality control metrics. Finally, it shows a practical example applying it to compare the performance of common imputation methods in bioinformatics (technically clearance or denoising methods in mathemtatics).

# Installation

The repository uses widely known python packages for the preprocessing, mainly pandas and scanpy and a `src` folder has been added containing the algorithms for the imputation methods. For the "Sinkhorn" algorithm (last practical part of the tutorail) a GPU is quite neccesary since the Optimal Transport algorithms require a large ammount of memory. For the pre-processing steps a CPU should be more than enough. To correctly run the code, I suggest using a virtual environment (not neccesarly conda) to avoid version compatibilities.<br>

Clone the repository by choosing a destination path (like your documents) and run the commands below. The repository will be cloned to `[path to repository]/rna-sequencing`.
```
$ cd [path to repository]
$ git clone https://github.com/lucas-rdlr/rna-sequencing.git
```
If https cloning does not work any more clone it via ssh (be sure to have ssh validation activated).

```
$ python -m venv [path to environment]/[name of environment]
```

Activate the environment before installing dependencies. In Linux:
```
$ source [path to environment]/[name of environment]/bin/activate
```

Lastly, you can install dependencies from the `requirements.txt` via:
```
$ pip install -r [path to repository]/rna-sequencing/requirements.txt
```

# Outline

 - `src` contatins all the `.py` modules for the imputation methods.
 - `notebooks` contains the `.ipynb` files and `.html` compiled version of the tutorial and experiments.
 - `requirements.txt` contains the python packages needed to run the notebooks.
