# 2025 Microscopy & Microanalysis HyperSpy Workshop

Training material used during the 2025 HyperSpy Workshop at the Microscopy and Microanalysis meeting in Salt Lake City, UT
in the short course _X-10 EM Data Analysis with the HyperSpy Ecosystem_.

## ✨ Try it in your browser ✨

While we recommend downloading this repository and running the code locally (since that will be how you use
HyperSpy on your own data), you can use the following link to interactively run these tutorial files
in your web browser during the course.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hyperspy/MM2025_HyperSpy_Workshop/HEAD)

Otherwise, follow the [Software Installation](#software-installation) section to download the files and install HyperSpy.

## Venue

Room 151 A, Salt Palace Convention Center, Salt Lake City, UT. 

## Agenda

The workshop will take place from 8:30 to 17:00 MDT on Sunday the July 27, 2025. The program will officially
start at 8:45, but the instructors will be present from 8:00 onwards to assist anyone with installation issues
before the course begins.

| Time         | Length | Activity                                                                   | Presenter            |
|--------------|--------|----------------------------------------------------------------------------|----------------------|
| 8:30-8:45    | 15m    | Welcome / installation help                                                |                      |
| 8:45-9:00    | 15m    | Introduction talk                                                          | Josh Taillon         |
| 9:00-10:15   | 1h15m  | 1. Getting started / HyperSpy Basics                                       | Josh Taillon         |
| 10:15-10:30  | 15m    | Coffee break                                                               |                      |
| 10:30-11:15  | 45m    | 2. Decomposition and BSS                                                   | Josh Taillon         |
| 11:15-12:00  | 45m    | 3. Curve fitting                                                           | Carter Francis       |
| 12:00-12:45  | 45m    | 4. EDX with [eXSpy](https://hyperspy.org/exspy/)                           | Carter Francis       |
| 12:45-13:30  | 45m    | Lunch break                                                                |                      |
| 13:30-14:15  | 45m    | 5. EELS with [eXSpy](https://hyperspy.org/exspy/)                          | Josh Taillon         |
| 14:15-15:00  | 45m    | 6. Cathodoluminescence with [LumiSpy](https://docs.lumispy.org)            | Josh / Carter        |
| 15:00-15:30  | 30m    | Coffee break                                                               |                      |
| 15:30-16:15  | 45m    | 7. Lazy signals for Big Data                                               | Carter Francis       |
| 16:15-17:00  | 45m    | 8. 4D-STEM with [Pyxem](https://pyxem.readthedocs.io/en/stable/index.html) | Carter Francis       |

The numbered activities correspond to the tutorials in the folders of this repository.

## Instructors

- Joshua Taillon ([DataSophos, LLC](https://datasophos.co))
- Carter Francis (Direct Electron)
- Tina Bergh (NTNU) 
- Nick Hagopian (UW Madison)
- Geri Topore (Imperial College London)

## Downloading large files

> [!CAUTION]
> This needs to be updated

Download the zip-file from this link: https://filesender.sikt.no/?s=download&token=000ee6a7-008e-4a63-aada-67706ef762bc

## Software installation

To use the Jupyter Notebooks in this repository, you need to install some software packages first. Installation instructions for beginners and advanced users can be found below.


### Simple installation instructions (best for Python beginners)

The easiest way to install all the software required to run the Jupyter Notebooks in this repository is to [install the HyperSpy Bundle](https://hyperspy.org/hyperspy-bundle/install.html), which can be downloaded from [here](https://github.com/hyperspy/hyperspy-bundle/releases/latest).


### Advanced installation instructions (for advanced users)

If you prefer to customize your installation, we suggest installing a conda distribution (we suggest [MiniForge](https://github.com/conda-forge/miniforge)) and install all the required Python packages in a dedicated environment executing the following commands in a terminal (the conda prompt in Windows):


```bash
conda install nb_conda_kernels jupyterlab start_jupyter_cm ipympl -c conda-forge
conda create -n hyperspy_MM2025 python=3.11 hyperspy pyxem ipympl exspy lumispy ipykernel -c conda-forge
```

To use HyperSpy in JupyterLab, start Jupyter Lab and choose the `Python [conda env:hyperspy_MM2025]` kernel. Alternatively, start JupyterLab from the `hyperspy_MM2025` environment as follows:

```bash
conda activate hyperspy_MM2025
jupyter lab
```
