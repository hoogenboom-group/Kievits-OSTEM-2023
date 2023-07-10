# Single beam optical STEM demonstration 
Arent Kievits, 05-05-2021

This repository holds code and data for analysis of single beam optical scanning transmission electron microscopy (Optical STEM / OSTEM), a novel detection method for scanning electron microscopy. It serves as a place to manage the code and demonstrate the findings of the research via an easy to set up and interactive Jupyter notebook environment.

### Installation

It is recommended (and currently only supported) to install this repository with `conda` (https://docs.conda.io/en/latest/miniconda.html) via the command line. Install `miniconda` first and then open the terminal. In Windows, search for `anaconda prompt` in the search bar and in Mac OS search for `terminal` in the finder. Enter the following commands in the terminal:

* Install `git` with `conda` to be able to clone the GitHub repository
```bash
conda install git
```

* Clone GitHub repository into suitable directory
```bash
git clone https://github.com/arentkievits/sb_optical_STEM
```

* Create and activate new `conda` environment called `ostem-demo`
```bash
conda env create --file=environment.yml
conda activate ostem-demo
```

* Install package from GitHub
```bash
pip install git+git://github.com/arentkievits/ostem
```

### Use

The main code is contained in the `DEMO_Optical_STEM.ipynb` file, which is an interactive Jupyter notebook for viewing the data and plotting the results. To start the environment, use the command line to get to the `git` folder and type `jupyter lab` or search `jupyter notebook` via the Windows/Mac programs tab and go to the respective repository location.

The notebook can be executed at once by hitting the `play` button or by selecting `Run` > 'Run All Cells'

### /DEMO_data
Folder that contains the experimental data

* `SNR_comparison_final` -- Backscatter electron images acquired with the CBS detector (BSE), Secondary electron images acquired with the through-the-lens detector (SE), backscatter electron images acquired with stage bias (BSE-SB) and optical STEM images acquired with the photon detector (OSTEM). 5 images per setting.

| Detection mode | LE (eV) | Dwell (ns) | Pixel size (nm/px) |
|:--------------:|:-------:|:----------:|:------------------:|
| BSE<br>BSE-SB<br>SE<br>OSTEM | 1500 (BSE, BSE-SB, SE)<br>4000 (OSTEM) | 100<br>200<br>300<br>500<br>1000<br>3000<br>5000<br>10000 | 1 |

* `Optimization_OSTEM` -- Optical STEM images acquired with the photon detector (OSTEM). 5 images per setting.

| LE (keV) | Dwell (ns) | Pixel size (nm/px) |
|:--------:|:----------:|:------------------:|
| 2.5<br>3.0<br>3.5<br>4.0<br>4.5<br>5.0<br>5.5<br>6.0<br>6.5<br>7.0<br>7.5<br>8.0| 0<br>100<br>200<br>500<br>1000<br>1500<br>2000<br>3000 | 100<br>200<br>300<br>500<br>1000<br>3000<br>5000<br>10000 | 1 |

### /code
Contains the code used in the Demo notebook

### /Notebooks
Additional notebooks that are used for data analysis

