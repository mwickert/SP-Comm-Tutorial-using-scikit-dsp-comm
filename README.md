# SP-Comm Tutorial using *scikit-dsp-comm*

A tutorial on signal processing and communications using `scikit-dsp-comm`, including hardware interfacing to a software defined radio (SDR) and the PC audio subsystem. 

------

**Note**: To immediately jump into OS specific hardware and software configuration [visit the wiki pages](https://github.com/mwickert/SP-Comm-Tutorial-using-scikit-dsp-comm/wiki), but I suggest cloning the repo before you start setting up any hardware drivers, especially for Windows users.

```bash
git clone https://github.com/mwickert/SP-Comm-Tutorial-using-scikit-dsp-comm.git
```
------

## Introduction

This project provides the set-up instructions and content needed for the Scipy 2017 tutorial on signal processing and communications using the `scikit-dsp-comm` package. To get the most out of this tutorial you will want to take the time to install and configure both software and hardware interface drivers for the [RTL-SDR](http://www.rtl-sdr.com/) low-cost software defined radio platform and [Pyaudio](https://people.csail.mit.edu/hubert/pyaudio/).

## Getting Ready for the Tutorial

### Python Version and Packages

* Python 3.6 preferred, but Python 2.7 also works, as is the origin of scikit-dsp-comm
* I recommend using Anaconda as your Python base, its ability to use virtual environments
* * Note a virtual environment is however not included in the repo
* The following Scipy packages are required: `numpy`, `matplotlib`, `scipy`, `ipython`, `pyqt`, and `jupyter`, as well as related dependencies; with the full install of Anaconda you are good, less the packages you install under the hardware set-up
* PIP install (*pending* conda install) `scikit-dsp-comm`; this is preferred for the tutorial, but I will likely have the modules locally available in the folders where you will do hands-on work during the tutorial

### Cloning this Repo

* Clone this repo to some convenient location on your PC: `git https://github.com/mwickert/SP-Comm-Tutorial-using-scikit-dsp-comm.git`. This will place a directory structure for testing the hardware and also all the folders which contain the lecture material and Jupyter notebooks for hands-on exercises

![folder_layout](images/folder_layout.png)

* The lecture material and Jupyter notebooks are in development, and will appear over time as the conference approaches. The absolute newest version will be pushed just before the tutorial; using `git fetch` and/or `git pull` you will be see the changes and then them merge them with your local repo

### Setting Up Hardware Interfaces

* Visit the [Wiki pages](https://github.com/mwickert/SP-Comm-Tutorial-using-scikit-dsp-comm/wiki) and choose your operating system. Python packages related to the configuration will also be installed in this process
* At the end of the installation process you will have the opportunity to test you install using content from the `hardware_configuration` folder

