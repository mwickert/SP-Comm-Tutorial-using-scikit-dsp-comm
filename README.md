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

> **Newly added**: To drive signals into PyAudio you should have a 3.5 mm audio cable to interface  your cell phone to your PCs audio input jack (perhaps on an [external sound card](https://www.amazon.com/Sabrent-External-Adapter-Windows-AU-MMSA/dp/B00IRVQ0F8/ref=sr_1_3?s=electronics&ie=UTF8&qid=1499267425&sr=1-3&keywords=USB+audio) ) . Add to this a signal generator app for your cell phone. On the iPhone I like using (https://www.cateater.com/signalgenerator/). Screen shots of these items are at the bottom of this page.

## Getting Ready for the Tutorial

### Python Version and Packages

* Python 3.6 preferred, but Python 2.7 also works, as this is the origin of scikit-dsp-comm
* I recommend using Anaconda as your Python base, its ability to use virtual environments
* * Note a virtual environment is however not included in the repo
* The following Scipy packages are required: `numpy`, `matplotlib`, `scipy`, `ipython`, `pyqt`, and `jupyter`, as well as related dependencies; with the full install of Anaconda you are good, less the packages you install under the hardware set-up
* PIP install (*pending* conda install) `scikit-dsp-comm`
  * Option 1: Independent of having the repo cloned on your system you may `pip install scikit-dsp-comm1`; 
  * Option 2: With a bash shell, command prompt, or power shell sitting at the location of the clone  `pip install -e .`; This is known as an *editble install*, which means if you pull new versions in to the local repo you can quickly reinstall the changes. **This is recommended** for the tutorial, as updates may come on Monday evening or Tuesday morning of the conference. I will use *Slack* to alert you.
  * To import the package, or portions of it, use for example: `import sk_dsp_comm.sigsys as ss`

### Cloning this Repo

* Clone this repo to some convenient location on your PC: `git https://github.com/mwickert/SP-Comm-Tutorial-using-scikit-dsp-comm.git`. This will place a directory structure for testing the hardware and also all the folders which contain the lecture material and Jupyter notebooks for hands-on exercises

![folder_layout](images/folder_layout.png)

* The lecture material and Jupyter notebooks are in development, and will appear over time as the conference approaches. The absolute newest version will be pushed just before the tutorial; using `git fetch` and/or `git pull` you will be see the changes and then them merge them with your local repo

### Setting Up Hardware Interfaces

* Visit the [Wiki pages](https://github.com/mwickert/SP-Comm-Tutorial-using-scikit-dsp-comm/wiki) and choose your operating system. Python packages related to the configuration will also be installed in this process

* At the end of the installation process you will have the opportunity to test you install using content from the `hardware_configuration` folder


## Extra Pyaudio Interface Tools

![Cables and generator app](images/PyAudio_hardware_interconnect.png)  