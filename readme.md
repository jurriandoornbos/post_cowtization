<div align="center">
  <p>
    <a href="https://icaerus.eu" target="_blank">
      <img width="50%" src="https://raw.githubusercontent.com/ICAERUS-EU/.github/refs/heads/main/profile/ICAERUS_transparent.png"></a>
    <h3 align="center">Cowtization 🐄</h3>
    
   <p align="center">
    Code for ICAERUS blogpost on Deep Learning quantization using a trained cow detection model.
    <br/>
    <br/>
    <a href="https://github.com/jurriandoornbos/cowtization/wiki"><strong>Explore the wiki »</strong></a>
    <br/>
    <br/>
    <a href="https://github.com/jurriandoornbos/cowtization/issues">Report Bug</a>
    .
    <a href="https://github.com/jurriandoornbos/cowtization/issues">Request Feature</a>
  </p>
</p>
</div>

![Downloads](https://img.shields.io/github/downloads/jurriandoornbos/cowtization/total) ![Contributors](https://img.shields.io/github/contributors/jurriandoornbos/cowtizationcolor=dark-green) ![Forks](https://img.shields.io/github/forks/jurriandoornbos/cowtization?style=social) ![Stargazers](https://img.shields.io/github/stars/jurriandoornbos/cowtization?style=social) ![Issues](https://img.shields.io/github/issues/jurriandoornbos/cowtization) ![License](https://img.shields.io/github/licensejurriandoornbos/cowtization) 

## Table Of Contents

* [Summary](#summary)
* [Installation](#installation)
  
## Summary
The notebooks presented, as well as the model weights presents everything needed to run your own quantization experiments and training an SSDLite model using the [cow detection dataset from ICAERUS](https://zenodo.org/records/10245396).

## Installation:
You can choose to install everything in a Python virtual environment or directly run a jupyterlab docker:


##### Option A: Setup through Docker:
This starts a premade jupyter environment with everything preinstalled, based around a nvidia docker image for DL support.
* Linux/Ubuntu:
  ```bash
  docker run --rm -it --runtime=nvidia -p 8888:8888 --gpus 1 --shm-size=5gb --network=host -v /path_to_local/dir:/home/jovyan jurrain/drone-ml:gpu-torch11.8-uavgeoformers
  ```

`--network=host` flag whether you want to run it on a different machine in the same network, and want to access the notebook. (does not run locally)

`-v` flag makes sure that once downloaded, it stays in that folder, accessible from the PC, and when restarting, all the weights etc. remain in that folder. `path_to_local/dir` is thew path to your working dir where you want to access the notebook from. can be `.` if you already `cd`ed into it.

` --runtime=nvidia` can be skipped when working on WSL2



* Windows requires WSL2 and NVIDIA drivers, WSL2 should also have the nvidia toolkit (for deep learning)
